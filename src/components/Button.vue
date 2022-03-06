<template>
  <v-btn class="align-center justify-space-around ma-5">{{ text }}</v-btn>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: String,
  },
};
</script>
