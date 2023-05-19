<template>
  <v-list lines="three">
    <div>
      <v-avatar>
        <v-img src="https://cdn.vuetifyjs.com/images/john.jpg" alt="John"></v-img>
      </v-avatar>
    </div>
    <v-list-item prepend-avatar="https://cdn.vuetifyjs.com/images/john.jpg">
      <v-form>
        <v-text-field
          variant="plain"
          placeholder="What are you doing now?"
          persistent-placeholder
        ></v-text-field>
        <v-divider />
        <v-btn class="mt-4" color="primary">tweet</v-btn>
      </v-form>
    </v-list-item>
  </v-list>
</template>
