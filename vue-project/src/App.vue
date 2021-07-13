<template>
  <div id="nav">
    <router-link to="/">Home</router-link>
    <br>
    <router-link to="/databinding">Data Binding</router-link>
    <br>
    <router-link to="/databindinghtml">Data Binding Html</router-link>
    <br>
    <router-link to="/databindinginputtext">Data Binding InputText</router-link>
    <br>
    <router-link to="/databindingtextarea">Data Binding Textarea</router-link>
    <br>
    <router-link to="/databindingselect">Data Binding Select</router-link>
    <br>
    <router-link to="/databindingchecked">Data Binding Checked</router-link>
    <br>
    <router-link to="/databindingradio">Data Binding Radio</router-link>
    <br>
    <router-link to="/databindingimg">Data Binding Img</router-link>
    <br>
    <router-link to="/databindingbutton">Data Binding Button</router-link>
    <br>
    <router-link to="/databindingclass">Data Binding Class</router-link>
    <br>
    <router-link to="/databindinglist">Data Binding List</router-link>
  </div>
  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
</style>
