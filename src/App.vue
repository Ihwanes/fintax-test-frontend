<template>
  <v-app>
    <!-- Place to including the components that being used in this project to the base page -->
    <v-main>
      <AppBar />
      <HelloWorld />
      <v-container>
        <Hero />
        <Stuff />
        <h1>Skills</h1>
        <Table />
        <h1>Contact me</h1>
        <Contact />
      </v-container>
    </v-main>
  </v-app>
</template>

<script>
//Import the components
import HelloWorld from "./components/HelloWorld";
import Table from "./components/Table";
import Hero from "./components/Hero";
import Stuff from "./components/Stuff";
import Contact from "./components/Contact";
import AppBar from "./components/AppBar";

export default {
  name: "App",

  //List of all the components that being used in this project
  components: {
    HelloWorld,
    Table,
    Hero,
    Stuff,
    Contact,
    AppBar,
  },

  data: () => ({
    //
  }),
};
</script>
