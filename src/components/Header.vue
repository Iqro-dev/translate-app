<template>
  <v-app>
    <v-app-bar elevation="4" class="justify-center">
      <Button text="toggle theme" @click="$emit('toggleTheme')" />
      <h1>Translate</h1>
    </v-app-bar>
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
