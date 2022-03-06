<template>
  <v-layout :theme="theme">
    <v-app-bar>
      <Header />
    </v-app-bar>
    <v-main>
      <Main @toggleTheme="toggleTheme" />
    </v-main>
  </v-layout>
</template>

<script>
import { ref } from "vue";
import Header from "./Header.vue";
import Main from "./Main.vue";

export default {
  name: "Layout",
  components: {
    Header,
    Main,
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
