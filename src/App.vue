<template>
  <v-app>

    <!-- Create an app bar -->
    <v-app-bar app color="primary" dark>
      <div class="d-flex align-center">
        <v-avatar>
          <img src="../src/assets/my-foto-avatar.jpg" alt="Ihwanes Avatar" />
        </v-avatar>

        <span class="mr-2">Ihwanes</span>
      </div>

      <v-spacer></v-spacer>

      <v-btn
        href="https://github.com/vuetifyjs/vuetify/releases/latest"
        target="_blank"
        text
      >
        <span class="mr-2">Latest Release</span>
        <v-icon>mdi-open-in-new</v-icon>
      </v-btn>
    </v-app-bar>

    <!-- Place to including the components that being used in this project to the base page -->
    <v-main>
      <HelloWorld />
      <Table />
    </v-main>
  </v-app>
</template>

<script>

//Import the components
import HelloWorld from "./components/HelloWorld";
import Table from "./components/Table";

export default {
  name: "App",

  //List of all the components that being used in this project
  components: {
    HelloWorld,
    Table,
  },

  data: () => ({
    //
  }),
};
</script>
