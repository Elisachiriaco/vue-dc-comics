<template>
  <div id="app">
   <AppHeader />
   <AppGrid />
   <AppFooter />
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppGrid from './components/AppGrid.vue'
import AppFooter from './components/AppFooter.vue'

export default {
  name: 'App',
  components: {
    AppHeader,
    AppGrid,
    AppFooter,
  }
}
</script>

<style lang="scss">
@import './style/variables';
@import './style/generals';

</style>
