
<template>
  <v-card class="overflow-hidden">
    <v-card tile>
      <v-app-bar
        absolute
        color="#005b4e"
        shrink-on-scroll
        prominent
        dark
        scroll-target="#scrolling-techniques-4"
      >
        <v-app-bar-nav-icon></v-app-bar-nav-icon>

        <v-toolbar-title></v-toolbar-title>

        <v-spacer></v-spacer>

        <v-img
          :src="'/imgs/logo_BSR_with_Cynthia_ white_on_green.png'"
          max-height="128"
          max-width="200"
          contain
        ></v-img>

        <v-spacer></v-spacer>

        <template v-slot:extension>
          <v-tabs align-with-title background-color="transparent">
            <v-tab v-on:click.prevent="scrollToSection('home')">Home</v-tab>
            <v-tab v-on:click.prevent="scrollToSection('service')"
              >Service</v-tab
            >
            <v-tab v-on:click.prevent="scrollToSection('faq')">FAQ</v-tab>
            <v-tab v-on:click.prevent="scrollToSection('contact')"
              >Contact</v-tab
            >
            <v-tab v-on:click.prevent="scrollToSection('about')">About</v-tab>
          </v-tabs>
        </template>
      </v-app-bar>
      <v-sheet
        id="scrolling-techniques-4"
        class="overflow-y-auto"
        max-height="600"
      >
        <v-container style="height: 2000px"></v-container>
      </v-sheet>
    </v-card>
  </v-card>
</template>

<script>
export default {
  name: "playground",
  data: () => ({
    //
  }),
};
</script>
