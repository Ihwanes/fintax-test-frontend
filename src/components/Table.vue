<template>
  <v-container>
    Currently this is my Skills, will be added more of it for sure in the future, so keep it up!
    <v-card>
      <v-card-title>
        Skills
        <v-spacer></v-spacer>
        <v-text-field
          v-model="search"
          append-icon="mdi-magnify"
          label="Search"
          single-line
          hide-details
        ></v-text-field>
      </v-card-title>
      <v-data-table
        :headers="headers"
        :items="skills"
        :search="search"
      ></v-data-table>
    </v-card>
  </v-container>
</template>
<script>
export default {
  data() {
    return {
      search: "",
      headers: [
        { text: "Name", value: "name" },
        { text: "Proficiency (1-10)", value: "proficiency" },
        { text: "Field", value: "field" },
      ],
      skills: [
        {
          name: "Django",
          proficiency: 7.5,
          field: "Backend Development",
        },
        {
          name: "Figma",
          proficiency: 7.5,
          field: "UI/UX",
        },
        {
          name: "Java",
          proficiency: 6.5,
          field: "Software Development",
        },
        {
          name: "Agile/Scrum",
          proficiency: 7.5,
          field: "Software Development"
        },
        {
          name: "English",
          proficiency: 7.5,
          field: "Language"
        },
        {
          name: "Vue.js",
          proficiency: 6,
          field: "Frontend Development"
        },
        {
          name: "User Research",
          proficiency: 7,
          field: "UI/UX"
        },
        {
          name: "Adobe Illustrator",
          proficiency: 6.5,
          field: "Design"
        },
        {
          name: "Adobe Lightroom",
          proficiency: 6.5,
          field: "Design"
        },
        {
          name: "Git",
          proficiency: 7,
          field: "Software Development"
        },
      ],
    };
  },
};
</script>