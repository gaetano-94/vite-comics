<script>
import AppFooterList from './AppFooterList.vue';
import AppSocialIcon from './AppSocialIcon.vue';
export default {
  name: 'Footer',
  components: {
    AppFooterList,
    AppSocialIcon,
  },
};
</script>

<template>
  <footer>
    <AppFooterList />
    <AppSocialIcon />
  </footer>
</template>

<style scoped></style>
