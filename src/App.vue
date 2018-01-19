<template>
  <div id="app">
    <b-container fluid>
    <b-row>
      <information/>
    </b-row>
    <b-row>
      <imageGrid class="grid" />
    </b-row>
    <b-row>
      <FAQ/>
    </b-row>
    <b-row class="closing" style="padding: 1rem;">
      &copy; Anouk Boukema
    </b-row>
    </b-container>
  </div>
</template>

<script>
import ImageGrid from './components/ImageGrid'
import Information from './components/Information'
import FAQ from './components/FAQ'
import 'bootstrap/dist/css/bootstrap.css'
import 'bootstrap-vue/dist/bootstrap-vue.css'
export default {
  name: 'app',
  components: {
    Information,
    ImageGrid,
    FAQ
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
}

.grid{
  margin-top: 50px;
}

/* .row{
  padding-top: 50px;
} */

.closing{
  padding-top: 0;
  background-color: #5C5FA1;
}
</style>
