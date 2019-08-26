<template>
  <div class="aid-section">
      <div class="aid-section-header">
        <div class="aid-section-header-text">How Those it work?</div>
        <div class="aid-section-header-line"></div>
      </div>
  </div>
</template>

<script>

export default {
  name: 'aidSection',
  components: {

  }
}
</script>
<style scoped>
.aid-section {
  width: 100%;
}
.aid-section .aid-section-header {
  text-align: center;
  font-size: 25px;
  margin-top: 100px;
}
.aid-section .aid-section-header-line{
  height: 10px;
  width: 60px;
  background-color: var(--red);
  margin-left: auto; 
  margin-right: auto;
  margin-top: 20px;
  border-radius: 30px;
}
</style>