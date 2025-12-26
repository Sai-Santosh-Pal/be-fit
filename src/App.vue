<script setup>
  import Welcome from './components/pages/Welcome.vue'
  import Layout from './components/layouts/Layout.vue'
  import Dashboard from './components/pages/Dashboard.vue'
  import Workout from './components/pages/Workout.vue'

const selectDisplay = 3
</script>

<template>
  <Layout>
    <Welcome v-if="selectDisplay == 1" />
    <Dashboard v-if="selectDisplay == 2" />
    <Workout v-if="selectDisplay == 3" />
  </Layout>
</template>

<style scoped>

</style>
