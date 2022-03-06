<template>
  <Button text="toggle theme" @click="$emit('toggleTheme')" />
  <v-main></v-main>
</template>

<script>
import Button from "./Button.vue";

export default {
  name: "Main",
  components: {
    Button,
  },
};
</script>
