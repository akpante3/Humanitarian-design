<template>
  <div class="aid-section">
      <div class="section-header">
        <br>
        <div class="section-header-text">How Those it work?</div>
        <div class="section-header-line"></div>
        <br>
      </div>
      <div class="aid-section-options">
        <!-- aid-icons -->
        <div class="aid-section-icons"> 
          <div>
            <i class="fas fa-user-plus fa-3x"></i>
          </div>
          <div>
            <i class="fas fa-boxes fa-3x"></i>
          </div>
          <div>
            <i class="fas fa-donate fa-3x"></i>
          </div> 
        </div>
        <!-- aid-option-list -->
        <div class="aid-options-list">
          <div class="options-list" v-for="option in optionList" :key="option.number">
             <span class="option-list-num">{{option.number}}</span>
             <div class="option-description">
               <div class="option-description-header">
                 {{option.header}}
               </div>
               <div class="option-description-text">
                 {{option.text}}
               </div>
             </div>
          </div>
        </div>
      </div>
  </div>
</template>

<script>

export default {
  name: 'aidSection',
  data () {
    return {
      optionList: [
        {number: 1, header: 'Join', text: 'Lorem ipsum dolor sit amet consectetur adipisicing.'},
        {number: 2, header: 'Select', text: 'Lorem ipsum dolor sit amet consectetur adipisicing.'},
        {number: 3, header: 'Donate', text: 'Lorem ipsum dolor sit amet consectetur adipisicing.'}
      ]
    }
  },
  components: {

  }
}
</script>
<style lang="scss">
@import '../../assets/style/style.css';

.aid-section {
  width: 100%;
  height: 450px;
  .aid-section-options {
    display: grid;
    grid-template-rows: 1fr;
    margin-top: 50px;
  }
  .aid-section-icons {
    width: 80%;
    margin: 0 auto;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
  }
  .aid-section-icons div {
    color: #f15e31;
    text-align: center;
  }
  .aid-options-list {
    width: 80%;
    margin-left: auto;
    margin-right: auto;
    margin-top: 30px;
    display: grid;
    grid-template-columns: 1fr 1fr 1fr;
  }
  .options-list {
    display: grid;
    grid-template-columns: 0.5fr 1.5fr;
  }
  .options-list .option-list-num {
    text-align: right;
    font-size: 75px;
    font-weight: 1000;
    color: #f0f0f0;
  }
  .options-list .option-description {
    padding: 12px;
  }
}
</style>