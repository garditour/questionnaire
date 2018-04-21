<template>
  <div id="app">
    <b-container>
      <header class="my-5 pb-4 border-bottom d-flex justify-content-between">
        <h1><i class="material-icons" style="font-size:36pt">assessment</i> Questionnaire</h1>
        <b-nav pills class="d-flex justify-content-center"> 
          <b-nav-item active><i class="material-icons">add</i> Add Questionnaire</b-nav-item>
          <b-nav-item><i class="material-icons">multiline_chart</i> Show Report</b-nav-item>
        </b-nav>
      </header>
      <router-view></router-view>
    </b-container>
  </div>
</template>

<script>
export default {
  name: 'App'
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
.nav-item a {
  border-radius: 50px !important;
}
.material-icons{
    display: inline-flex;
    vertical-align: top;
}
</style>
