<script>
import AppMainTop from './AppMainTop.vue';
import AppMainBottom from './AppMainBottom.vue';
export default {
  name: 'Main',
  components: {
    AppMainTop,
    AppMainBottom,
  },
};
</script>

<template>
  <main>
    <AppMainTop />
    <AppMainBottom />
  </main>
</template>

<style scoped lang="scss">
@use '../styles/partials/variables..scss' as *;
</style>
