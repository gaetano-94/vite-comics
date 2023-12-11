<script>
import AppMainTop from './AppMainTop.vue';
import AppMainBottom from './AppMainBottom.vue';
import AppMainBlueBar from './AppMainBlueBar.vue';
export default {
  name: 'Main',
  components: {
    AppMainTop,
    AppMainBottom,
    AppMainBlueBar,
  },
};
</script>

<template>
  <main>
    <AppMainTop />
    <AppMainBottom />
    <AppMainBlueBar />
  </main>
</template>

<style scoped lang="scss">
@use '../styles/partials/variables..scss' as *;
</style>
