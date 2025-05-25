<template>
  <v-app>
    <v-app-bar app color="primary" dark>
      <v-toolbar-title>My App</v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn to="/" text>Home</v-btn>
      <v-btn to="/login" text>Login</v-btn>
    </v-app-bar>
    <router-view />
  </v-app>
</template>

<script setup>
  //
</script>
