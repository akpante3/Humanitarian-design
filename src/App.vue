<template>
  <div id="app">
    <div class="app-nav">
      <NavBar />    
    </div>
    <router-view></router-view>
  </div>
</template>

<script>
import NavBar from '@/components/ui/NavBar.vue'

export default {
  name: 'app',
  components: {
    NavBar
  }
}
</script>

<style>

body {
  margin: 0px;
  font-family: 'Varela Round', sans-serif;
}
div {
  box-sizing: border-box;
}
:root {
  --red: #f53123;
  --dark-red: #a72f27;
  --box-shadow: 1px 2px 20px 15px rgba(53, 53, 53, 0.2);
}
.app-nav {
  position: absolute;
  top: 0;
  width: 100%;
  z-index: 2;
}
.app {
  position: relative;
}
</style>
