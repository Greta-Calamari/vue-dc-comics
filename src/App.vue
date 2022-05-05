<template>
  <div id="app">
    <header>
    <AppHeader/>
    </header>
    <main>
    <AppJumbotron/>
    <AppMain/>
    <AppCard/>

    </main>

    <footer>
    <AppFooter/>


    </footer>

  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue'
import AppMain from './components/AppMain.vue'
import AppFooter from './components/AppFooter.vue'
import AppJumbotron from './components/AppJumbotron.vue'
import AppCard from './components/AppCard.vue'







export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    AppFooter,
    AppJumbotron,
    AppCard,
    
  }
}
</script>

<style lang="scss">
@import 'components/style/variables';
@import 'components/style/generals';

</style>
