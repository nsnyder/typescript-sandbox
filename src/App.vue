<template>
  <div id="app">
    <test-me />
    <test-me-again />
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import TestMe from "./test-me.vue";
import TestMeAgain from "./test-me-again.vue";

export default Vue.extend({
  name: "App",

  components: {
    TestMe,
    TestMeAgain
  }
});
</script>
