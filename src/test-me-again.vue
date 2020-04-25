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
export default {
  name: "TestMe",

  data() {
    return {
      truthy: true,
      thing: "I'm a thing!"
    };
  }
};
</script>
