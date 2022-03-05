<template>
  <v-app :theme="theme">
    <v-main>
      <Header @toggleTheme="toggleTheme" />
    </v-main>
  </v-app>
</template>

<script>
import Header from "./components/Header.vue";

import { ref } from "vue";

export default {
  name: "App",

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
