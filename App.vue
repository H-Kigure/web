<template>
  <div id="app">
    <header>
      <HeaderComponent></HeaderComponent>
    </header>
    <main class="mainWrap">
      <FirstView></FirstView>
      <router-view/>
    </main>
    <footer>
      <FooterComponent></FooterComponent>
    </footer>
  </div>
</template>

<script>
import HeaderComponent from './components/HeaderComponent'
import FooterComponent from './components/FooterComponent'
import FirstView from './components/FirstView'
export default {
  name: 'App',
  components: {
    HeaderComponent,
    FooterComponent,
    FirstView
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  min-height:800px;
}
header{
  position: sticky;
}
</style>
