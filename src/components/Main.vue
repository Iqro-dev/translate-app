<template>
  <Button text="toggle theme" @click="$emit('toggleTheme')" />
  <v-form>
    <v-container class="d-flex flex-row">
      <v-row>
        <v-col cols="12" sm="6">
          <v-text-field
            label="Input"
            clearable
            variant="outlined"
            class="pa-10"
            v-model="text"
            clear-icon="mdi-delete"
          ></v-text-field>
        </v-col>
        <v-col cols="12" sm="6">
          <v-text-field
            :label="this.text ? this.text : 'Text will appear here...'"
            clearable
            variant="contained"
            class="pa-10"
            disabled
          ></v-text-field>
        </v-col>
      </v-row>
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
  emits: ["toggleTheme"],
  data() {
    return {
      text: "",
    };
  },
};
</script>
