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
:root {
  --red: #f53123;
  --ligth-red: #ff746b;
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
