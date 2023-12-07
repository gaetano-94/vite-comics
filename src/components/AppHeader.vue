<script>
import AppLogo from './AppLogo.vue';
import AppNavbar from './AppNavbar.vue';
export default {
  name: 'Header',
  components: {
    AppLogo,
    AppNavbar,
  },
};
</script>

<template>
  <header>
    <AppLogo />
    <AppNavbar />
  </header>
</template>

<style scoped lang="scss">
@use '../styles/partials/variables..scss' as *;

header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  height: 120px;
  width: 1270px;
  margin: 20px auto;
}
</style>
