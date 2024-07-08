<template>
  <router-view />
  <v-layout>
    <v-app-bar>
      <v-app-bar-title> AM store</v-app-bar-title>

      <v-text-field
        prepend-icon="mdi-magnify"
        variant="solo"
        single-line
        density="compact"
        flat
        name="name"
        label="Search"
        class="mt-6 hidden-sm-and-down"
      ></v-text-field>
      <div class="hidden-sm-and-down">
        <v-btn variant="tonal">Home</v-btn>
        <v-btn variant="solo">About</v-btn>
        <v-btn variant="solo">Help</v-btn>
      </div>
      <v-spacer></v-spacer>
      <v-btn
        class="hidden-sm-and-down"
        color="success"
        append-icon="mdi-download"
        >Download App</v-btn
      >
      <v-btn class="hidden-sm-and-down" color="success" append-icon="mdi-login"
        >login</v-btn
      >
      <v-app-bar-nav-icon
        @click="open"
        class="hidden-md-and-up"
      ></v-app-bar-nav-icon>
    </v-app-bar>
    <v-navigation-drawer
      elevation-5
      v-model="this.nv"
      class="hidden-md-and-up pt-6 pl-3"
      width="200"
    >
      <v-list>
        <v-list-item
          append-icon="mdi-home"
          title="Home"
          value="home"
          color="success"
        ></v-list-item>
        <v-list-item
          append-icon="mdi-alert-circle-outline"
          title="About"
          value="About"
          color="success"
        ></v-list-item>
        <v-list-item
          append-icon="mdi-help"
          title="Help"
          value="Help"
          color="success"
        ></v-list-item>
      </v-list>
      <v-btn color="success" append-icon="mdi-download" variant="outlined"
        >Download App</v-btn
      >
      <v-btn
        color="success"
        append-icon="mdi-login"
        variant="outlined"
        class="mt-3"
        >login</v-btn
      >
      <v-text-field
        prepend-icon="mdi-magnify"
        variant="solo"
        single-line
        density="compact"
        flat
        name="name"
        label="Search"
        class="mt-6"
      ></v-text-field>
    </v-navigation-drawer>
  </v-layout>
</template>

<script setup></script>

<script>
export default {
  name: "App",
  data: () => {
    return {
      nv: false,
    };
  },
  methods: {
    open: function () {
      if (this.nv == false) {
        this.nv = true;
      } else {
        this.nv = false;
      }
    },
  },
};
</script>

<style scoped></style>
