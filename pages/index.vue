<template>
  <v-container>
    <v-row>
      <v-col v-for="personaje in $store.state.personajes" :key="personaje.id">
        <Card :personajes ="personaje" />
      </v-col>
    </v-row>
  </v-container>
</template>
<script>
import Card from '../components/Card.vue'
export default {
  components: {
    Card
  }
}
</script>
