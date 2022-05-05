<template>
  <div id="app">
    <header>
    <AppHeader/>
    </header>
    <main>
    <AppJumbotron/>
    <AppMain/>

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




export default {
  name: 'App',
  components: {
    AppHeader,
    AppMain,
    AppFooter,
    AppJumbotron,
  }
}
</script>

<style lang="scss">
@import 'components/style/variables';
@import 'components/style/generals';

</style>
