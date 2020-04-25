<template>
  <div id="app">
    <test-me />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import { ref } from "@vue/composition-api";
import TestMe from "./test-me.vue";

export default Vue.extend({
  name: "App",

  components: {
    TestMe
  },
  setup() {
    const truthy = ref(true);
    const thing = ref("I'm a thing!");
    return {
      thing,
      truthy
    };
  }
});
</script>
