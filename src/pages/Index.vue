<template>
  <q-page class="column flex-center">
    <h2>Rental Calculator</h2>
    <q-select
      :options='seasonOptions'
      v-model='season'
    />
    <q-select
      :options='locationOptions'
      v-model='location'
    />
    <q-select
      :options='vehicleOptions'
      v-model='vehicle'
    />
    <!-- <p>{{ options }}</p> -->
  </q-page>
</template>

<style>
</style>

<script>
import allRates from '../data/rates';
import { options } from '../data/options';

export default {
  name: 'PageIndex',
  data: function () {
    return {
      allRates,
      days: 0,
      season: 'Season',
      vehicle: 'Vehicle',
      location: 'Location',
      seasonOptions: options.seasons,
      vehicleOptions: options.vehicles,
      locationOptions: options.locations
    }
  },
  methods: {

  }
}
</script>
