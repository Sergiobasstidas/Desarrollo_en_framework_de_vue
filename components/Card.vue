<template>
  <v-hover v-slot="{ hover }">
    <v-card class="mx-auto" :elevation="hover? 12 : 2" >
      <v-img :src="personajes.imagen"></v-img>
      <v-card-title>{{ personajes.nombre }}</v-card-title>
    </v-card>
  </v-hover>
</template>

<script>
export default {
  props: {
    personajes: {
      type: Object,
      required: true,
    },
  },
}
</script>

<style>
.v-card {
    transition: all 0.2s linear;
}
</style>
