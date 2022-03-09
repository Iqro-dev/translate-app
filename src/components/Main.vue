<template>
  <Button text="toggle theme" @click="$emit('toggleTheme')" />
  <v-form>
    <v-container class="d-flex flex-row">
      <v-text-field label="Input" clearable class="pa-10"></v-text-field>
      <v-text-field label="Input" clearable class="pa-10"></v-text-field>
    </v-container>
  </v-form>
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
