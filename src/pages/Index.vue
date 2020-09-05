<template>
  <div class="q-pa-md row items-start q-gutter-md">
    <div class="row">
      <div class="col col-md-4 col-sm-12" v-for="personaje in personajes" :key="personaje.id">
        <q-card class="my-card">
          <q-card-section>
            <img :src="personaje.imagen">
          </q-card-section>
          <q-card-section>
            <q-car-title>{{ personaje.nombre }}</q-car-title>
          </q-card-section>
        </q-card>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'PageIndex',
  data () {
    return {
      personajes: [
        {
          id: 1,
          nombre: 'Morty',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/2.jpeg'
        },
        {
          id: 2,
          nombre: 'Rick',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/1.jpeg'
        },
        {
          id: 3,
          nombre: 'Summer',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/3.jpeg'
        },
        {
          id: 4,
          nombre: 'Beth',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/4.jpeg'
        },
        {
          id: 5,
          nombre: 'Jerry',
          imagen: 'https://rickandmortyapi.com/api/character/avatar/5.jpeg'
        }
      ]
    }
  }
}
</script>
