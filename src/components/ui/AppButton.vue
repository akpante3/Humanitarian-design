<template>
    <div class="app-button">
      {{ title }}
    </div>
</template>

<script>
export default {
  name: 'LandingPage',
  components: {},
  data() {
    return {};
  },
  props:['title']
};
</script>

<style scoped>
.app-button {
  cursor: pointer;
  border-radius: 30px;
	font-size: 16px;
	border: none;
	transition: all 0.5s ease 0s;
  background-color: var(--red);
  width: 100px;
  text-align: center;
  padding: 10px;
  color: white;
  transition: 0.6;
}
.app-button:hover {
  background-color: var(--dark-red);
  font-weight: 900;
}

</style>