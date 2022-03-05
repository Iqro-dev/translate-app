<template>
  <v-app>
    <h1>Translate</h1>
    <Button text="toggle theme" @click="$emit('toggleTheme')" />
    <Button text="translate" />
  </v-app>
</template>

<script>
import Button from "./Button.vue";

export default {
  name: "Header",
  components: {
    Button,
  },
};
</script>

<style scoped>
h1 {
  text-align: center;
}
</style>
