<template>
  <!-- Create an app bar -->
  <v-app-bar app color="primary" dark>
    <div class="d-flex align-center">
      <v-avatar>
        <img src="../assets/my-foto-avatar.jpg" alt="Ihwanes Avatar" />
      </v-avatar>

      <v-spacer></v-spacer>
      <div class="font-weight-medium" style="margin: 1em">
        <span class="mr-2">Ihwanes</span>
      </div>
    </div>

    <v-spacer></v-spacer>

    <div class="text-center">
      <v-menu offset-y>
        <template v-slot:activator="{ on, attrs }">
          <v-btn color="primary" dark v-bind="attrs" v-on="on">
            Contact
          </v-btn>
        </template>
        <v-list>
          <v-list-item v-for="(item, index) in items" :key="index">
            <v-list-item-title><a ref="item.link">{{ item.title }}</a></v-list-item-title>
          </v-list-item>
        </v-list>
      </v-menu>
    </div>
  </v-app-bar>
</template>

<script>
export default {
  data: () => ({
    items: [
      { title: "Gmail", link: "https://mail.google.com/mail/?view=cm&fs=1&tf=1&to=ihwan1999@gmail.com" },
      { title: "Gitlab", link: "https://gitlab.com/ihwanes" },
      { title: "Github", link: "https://github.com/Ihwanes"},
      { title: "LinkedIn", link: "https://www.linkedin.com/in/ihwan-e-556a34136/" },
      { title: "Details", link: "/contact "}
    ],
  }),
};
</script>