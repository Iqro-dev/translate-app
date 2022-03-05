<template>
  <v-app>
    <v-btn>{{ text }}</v-btn>
  </v-app>
</template>

<script>
export default {
  name: "Button",
  props: {
    text: String,
  },
};
</script>
