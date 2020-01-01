<template>
  <div class="landing-page">
    <div class="landing-page-section-1">
        <div class="image-area"></div>
        <div class="text-area">
          <div class="text">
            <span>
              Lorem ipsum dolor sit amet consectetur adipisicing elit.
              Adipisci fugiat minima maiores, ducimus nobis hic perferendis doloremque,
              cupiditate sint minus aspernatur.
            </span>
             <div class="text-button">
                <AppButton
                 title="Donate"
                />
             </div>
          </div>
        </div>
        <div class="landing-page-image">
          <img src="@/assets/african.png"/>
        </div>
    </div>
    <div class="landing-page-section-2">
      <AidSection />
    </div>
    <div class="landing-page-section-3">
      <PhoneSection />
    </div>
    <div class="landing-page-section-4">
      <DonationSection />
    </div>
  </div>
</template>

<script>
import AppButton from '@/components/ui/AppButton.vue';
import AidSection from './AidSection.vue';
import PhoneSection from './PhoneSection';
import DonationSection from './DonationSection';

export default {
  name: 'LandingPage',
  components: {
    AppButton,
    AidSection,
    PhoneSection,
    DonationSection
  },
  data() {
    return {};
  },
};
</script>

<style scoped>
.landing-page-section-1 {
  height: 700px;
  margin: 0px;
  display: grid;
  grid-template-columns: 0.8fr 1.2fr;
  position: relative;
}
.landing-page-section-1 .image-area {
  background-color: var(--red);
}
.landing-page-section-1 .landing-page-image {
  position: absolute;
  bottom: 0;
  right: 80%;
  height: 600px;
  overflow: hidden;
  pointer-events: none;
  animation: landingPageImage 1.5s ease forwards;
}
.landing-page-section-1 .landing-page-image img {
  height: 800px;
  -webkit-filter: grayscale(100%);
  filter: grayscale(100%) brightness(80%) contrast(110%);
  transform: scaleX(-1);
}

@keyframes landingPageImage  {
  0%{ right: 80% }
  100%{ right: 40% }
}
.landing-page-section-1 .text-area {
  width: 100%;
  position: relative;
}
.landing-page-section-1 .text {
  width: 55%;
  font-size: 20px;
  position: absolute;
  top: 40%;
  left: 0; 
  right: 0; 
  margin-left: auto; 
  margin-right: auto;
}
.landing-page-section-1 .text span {
  line-height: 1.8;
}
.landing-page-section-1 .text-button {
  margin-top: 20px;
}
</style>
