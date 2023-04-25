<script setup lang="ts">
import { useRouter } from 'vue-router';

const router = useRouter();

const onCreate = () => router.push({ name: 'login' });
</script>

<template>
  <v-card class="ma-auto pa-15" width="600">
    <h1 class="signup-title">Create New Account</h1>
    <v-text-field class="mt-8" label="Name" variant="outlined" hide-details="auto"></v-text-field>
    <v-text-field
      class="mt-4"
      label="Password"
      variant="outlined"
      hide-details="auto"
    ></v-text-field>
    <v-btn block color="primary" class="mt-8" @click="onCreate">CREATE</v-btn>
  </v-card>
</template>

<style scoped lang="scss">
.signup-title {
  text-align: center;
}
</style>
