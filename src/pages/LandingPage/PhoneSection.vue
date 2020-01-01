<template>
  <div class="phone-section">
    <br>
    <div class="section-header">
      <div class="section-header-text">Give it a shot</div>
      <div class="section-header-line"></div>
    </div>
    <div class="card-holder">
      <div class="card-body">
        <img src="@/assets/phone.png"/>
        <div class="card-1 card"></div>
        <div class="card-2 card"></div>
        <div class="card-3 card"></div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  name: 'phoneSection',
  data () {
    return {
    }
  },
  components: {

  }
}
</script>
<style lang="scss">
.phone-section {
  height: 550px;
  background-color: #fafafa;
  position: relative;
  .card-body {
  width: 900px;
  height: 400px;
  position: relative;
  overflow: hidden;
  }
  .card-holder {
    display: inline-block;
    width: 900px;
    position:absolute;
    bottom: 0;
    left: 0; 
    right: 0; 
    margin-left: auto; 
    margin-right: auto;

  }
  .card-body img {
    width: 300px;
    position: absolute;
    z-index: 3;
    right: 90;
    top: 0;
  }
  .card {
    position: absolute;
    margin-top: auto;
    margin-bottom: auto;
    margin-left: 3%;
    bottom: 0; 
    top:0;
    border-radius: 5px;
    box-shadow: 1px 2px 8px 8px rgba(88, 88, 88, 0.1);
  }
  .card-1 {
    width: 91%;
    height: 80%;
    background-color: rgb(255, 255, 255);
    z-index: 2;
  }
  .card-2 {
    width: 93%;
    height: 70%;
    z-index: 1;
    background-color: none;
  }
  .card-3 {
    width: 95%;
    height: 60%;
    background-color: #fbfbfb;
  }
}
</style>