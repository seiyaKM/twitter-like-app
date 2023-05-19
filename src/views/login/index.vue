<script setup lang="ts">
import { useRouter } from 'vue-router';

const router = useRouter();

const onLogin = () => router.push({ name: 'home' });
</script>

<template>
  <v-card class="ma-auto pa-15" width="600">
    <h1 class="login-title">Login to Twitter Like</h1>
    <v-text-field
      class="mt-8"
      variant="outlined"
      placeholder="ID"
      hide-details="auto"
      persistent-placeholder
    ></v-text-field>
    <v-text-field
      class="mt-4"
      variant="outlined"
      placeholder="PASSWORD"
      hide-details="auto"
      persistent-placeholder
    ></v-text-field>
    <v-btn block color="primary" class="mt-8" @click="onLogin">LOGIN</v-btn>
    <p class="mt-4">
      don't have an account? Register <router-link :to="{ name: 'signup' }">here</router-link>
    </p>
  </v-card>
</template>

<style scoped lang="scss">
.login-title {
  text-align: center;
}
</style>
