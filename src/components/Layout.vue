<template>
  <v-app :theme="theme">
    <Header @toggleTheme="toggleTheme" />
  </v-app>
</template>

<script>
import { ref } from "vue";
import Header from "./Header.vue";

export default {
  name: "Layout",
  components: {
    Header,
  },
  setup() {
    const theme = ref("light");

    return {
      theme,
      toggleTheme: () =>
        (theme.value = theme.value === "light" ? "dark" : "light"),
    };
  },
};
</script>
