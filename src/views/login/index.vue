<template>
  <v-card class="ma-auto pa-15" width="600">
    <h1 class="login-title">TwitterLikeにログイン</h1>
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
    <v-btn block color="primary" class="mt-8">LOGIN</v-btn>
  </v-card>
</template>

<style scoped lang="scss">
.login-title {
  text-align: center;
}
</style>
