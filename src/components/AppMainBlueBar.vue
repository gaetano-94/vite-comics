<script>
export default {
  name: 'BlueBar',
};
</script>

<template>
  <div class="container">
    <ul class="container-img">
      <li class="img">
        <img src="/img/buy-comics-digital-comics.png" alt="" />
        <a href="#">
          <h3>Digital Comics</h3>
        </a>
      </li>
      <li class="img">
        <img src="/img/buy-comics-merchandise.png" alt="" />
        <a href="#">
          <h3>DC Merchandise</h3>
        </a>
      </li>
      <li class="img">
        <img src="/img/buy-comics-subscriptions.png" alt="" />
        <a href="#">
          <h3>Subscriptions</h3>
        </a>
      </li>
      <li class="img">
        <img src="/img/buy-comics-shop-locator.png" alt="" />
        <a href="#">
          <h3>Comic Shop Locator</h3>
        </a>
      </li>
      <li class="img">
        <img src="/img/buy-dc-power-visa.svg" alt="" />
        <a href="#">
          <h3>DC Power Visa</h3>
        </a>
      </li>
    </ul>
  </div>
</template>

<style scoped lang="scss">
@use '../styles/partials/variables..scss' as *;

.container {
  background-color: $secondary;
  padding: 40px;
  .container-img {
    max-width: 1260px;
    margin: 0px auto;
    display: flex;
    justify-content: space-between;

    .img {
      display: flex;
      justify-content: center;
      align-items: center;

      img {
        display: block;
        margin-right: 10px;
      }

      a {
        text-decoration: none;
      }
    }

    h3 {
      text-transform: uppercase;
      color: white;
      margin-right: 10px;
    }
  }
}
</style>
