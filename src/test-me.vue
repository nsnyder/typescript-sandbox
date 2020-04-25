<template>
  <div>
    <span v-if="truthy">
      This is all ok. ->
      {{ thing }}
    </span>

    <span v-if="truthy.test">
      This correctly errors!
    </span>

    <span v-if="truthier">
      This is wrong. ->
      {{ thingo }}
    </span>
  </div>
</template>

<script lang="ts">
import { ref, defineComponent } from "@vue/composition-api";

export default defineComponent({
  name: "TestMe",

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
