<template>
    <div class="nav-bar">
      <div class="nav-logo">Logo</div>
      <div class="nav-links">
        <ul>
          <li>Home</li>
          <li>FAQ</li>
          <li>Causes</li>
        </ul>
        <ul class="nav-auth">
          <li>Signup</li>
          <li>Login</li>
        </ul>
      </div>
    </div>
</template>

<script>
export default {
  name: 'LandingPage',
  components: {},
  data() {
    return {};
  },
};
</script>

<style scoped>
.nav-logo {
  padding: 10px;
}
.nav-bar {
  width: 100%;
  display: grid;
  grid-template-columns: 0.8fr 1.2fr;
}
.nav-links {
 width: 100%;
 text-align:  center;
}
.nav-bar ul {
 display: inline-block;
 box-sizing: border-box;
 height: 50px;
}
.nav-bar ul li {
  width: 80px;
  display: inline-block;
  margin-right: 5px;
  font-size: 18px;
  cursor: pointer;
  padding: 8px;
  transition: all 0.5s ease 0s;
  border-radius: 30px;
  border: 1px solid rgba(253, 0, 0, 0);
}
.nav-bar ul li:hover {
	border: 1px solid var(--red);
  color: var(--red);
}
</style>