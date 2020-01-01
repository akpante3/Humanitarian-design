<template>
  <div class="donation-section">
    <div class="donation-section-content">
      <div class="donation-cards">
        <div class="donation-card">
            <img src="https://www.mrguider.org/wp-content/uploads/2017/10/android-games-logo.jpg"/>
            <div class="option-description">
              <div class="donation-header">
                Header
              </div>
              <div class="donation-text">
                Lorem, ipsum dolor sit amet.
              </div>
            </div>
          </div>
          <div class="donation-card">
            <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRGq2BUxEz86BTLefTzaAVoZh2O6eK9IqMf2jyTGvEKaaXw44q8"/>
            <div class="option-description">
              <div class="donation-header">
                Header
              </div>
              <div class="donation-text">
                Lorem, ipsum dolor sit amet.
              </div>
            </div>
          </div>
          <div class="donation-card">
            <div class="donate-tag"></div>
            <img src="https://www.mrguider.org/wp-content/uploads/2017/10/android-games-logo.jpg"/>
            <div class="option-description">
              <div class="donation-header">
                Header
              </div>
              <div class="donation-text">
                Lorem, ipsum dolor sit amet.
              </div>
            </div>
          </div>
      </div>
      <div>
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Minus blanditiis deleniti porro.
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
.donation-section {
  width: 100%;
  height: 400px;
  background-color: #fafafa;
  padding-top: 50px;
  .donation-section-content {
    display: grid;
    grid-template-columns: 1fr 1fr;
    width: 60%;
    margin-right: auto;
    margin-left: auto;
    .donation-cards {
      display: grid;
      grid-template-rows: 1fr 1fr 1fr;
      grid-gap: 10px;
      width: 330px;
      height: 220px;
      box-sizing: border-box;
      .donation-card {
        width: 90%;
        height: 65px;
        display: grid;
        grid-template-columns: 0.5fr 1.5fr;
        background-color: #ffffff;
        padding: 10px;
        box-shadow: 1px 2px 4px 1px rgba(168, 168, 168, 0.2);
        margin: 0 auto;
        opacity: 0.5;
        position: relative;
        cursor: pointer;
        transition:  0.5s;
        box-sizing: border-box;
        .donate-tag {
          position: absolute;
          width: 50px;
          height: 20px;
          background-color: red;
          top: 10%;
          left: 86%;
          opacity: 0;
          transition:  0.5s;
        }
        .donation-text {
          font-size: 14px;
          transition:  0.5s;
        }
        .donation-header{
          font-weight: 900;
        }
        img {
          width: 50px;
          height: 50px;
          border-radius: 50%;
        }
      }
    .donation-card:hover {
      width: 95%;
      height: 70px;
      opacity: 1;
      .donation-text {
        font-size: 16px;
      }
      .donate-tag {
        opacity: 1;
      }
      img {
        width: 52px;
        height: 52px;
      }
    }
    }
  }

}
</style>