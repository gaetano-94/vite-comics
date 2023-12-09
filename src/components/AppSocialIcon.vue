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
    <div class="container-icon">
      <h2>Follow Us</h2>
      <ul class="container-img">
        <li>
          <a href="#">
            <img src="/img/footer-facebook.png" alt="" />
          </a>
        </li>
        <li>
          <a href="#">
            <img src="/img/footer-twitter.png" alt="" />
          </a>
        </li>
        <li>
          <a href="#">
            <img src="/img/footer-youtube.png" alt="" />
          </a>
        </li>
        <li>
          <a href="#">
            <img src="/img/footer-pinterest.png" alt="" />
          </a>
        </li>
        <li>
          <a href="#">
            <img src="/img/footer-periscope.png" alt="" />
          </a>
        </li>
      </ul>
    </div>
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

  .container-icon {
    display: flex;
    gap: 20px;
    justify-content: center;
    align-items: center;

    h2 {
      color: $secondary;
    }
  }

  .container-img {
    list-style-type: none;
    display: flex;
    gap: 20px;
    padding-right: 30px;
  }
}
</style>
