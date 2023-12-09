<script>
export default {
  name: 'SocialIcon',
};
</script>

<template>
  <div class="container-bottom">
    <div class="container-sing-up">
      <h2>
        <a href="#">Sing-Up Now!</a>
      </h2>
    </div>
    <div class="container-icon"></div>
  </div>
</template>

<style scoped lang="scss">
@use '../styles/partials/variables..scss' as *;
.container-bottom {
  display: flex;
  justify-content: space-between;
  align-items: center;
  background-color: $bg-footer-bt;
  margin: 0 auto;
  padding: 20px 30px;

  .container-sing-up {
    border: 2px solid $secondary;
    padding: 10px 20px;

    a {
      text-decoration: none;
      text-transform: uppercase;
      color: white;
      font-size: 20px;
    }
  }
}
</style>
