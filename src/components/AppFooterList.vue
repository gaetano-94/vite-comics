<script>
export default {
  name: 'FooterList',
  data() {
    return {
      dccomics: [
        {
          nome: 'Characters',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Comics',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Movie',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Tv',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Games',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Videos',
          link: '#',
          target: '_self',
        },
        {
          nome: 'News',
          link: '#',
          target: '_self',
        },
      ],
      dc: [
        {
          nome: 'Term of Use',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Privacy policy (New)',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Ad Choices',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Advertising',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Jobs',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Subscriptions',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Talent Workshops',
          link: '#',
          target: '_self',
        },
        {
          nome: 'CPSC Certificates',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Ratings',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Shop Help',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Contact Us',
          link: '#',
          target: '_self',
        },
      ],
      sites: [
        {
          nome: 'DC',
          link: '#',
          target: '_self',
        },
        {
          nome: 'MAD Megazine',
          link: '#',
          target: '_self',
        },
        {
          nome: 'DC Kids',
          link: '#',
          target: '_self',
        },
        {
          nome: 'DC Universe',
          link: '#',
          target: '_self',
        },
        {
          nome: 'DC Power Visa',
          link: '#',
          target: '_self',
        },
      ],
      shop: [
        {
          nome: 'Shop Dc',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Shop DC Collectibles',
          link: '#',
          target: '_self',
        },
      ],
    };
  },
};
</script>

<template>
  <div class="container-list">
    <div class="container-ul">
      <ul>
        <h2>Dc Comics</h2>
        <li v-for="list in dccomics">
          <a :href="list.link" :target="list.target">{{ list.nome }}</a>
        </li>
        <h2 class="shop">Shop</h2>
        <li v-for="list in shop">
          <a :href="list.link" :target="list.target">{{ list.nome }}</a>
        </li>
      </ul>

      <ul>
        <h2>Dc</h2>
        <li v-for="list in dc">
          <a :href="list.link" :target="list.target">{{ list.nome }}</a>
        </li>
      </ul>

      <ul>
        <h2>Sites</h2>
        <li v-for="list in sites">
          <a :href="list.link" :target="list.target">{{ list.nome }}</a>
        </li>
      </ul>
    </div>
    <div class="container-logo">
      <img src="/img/dc-logo-bg.png" alt="Logo-Big-Dc" />
    </div>
  </div>
</template>

<style scoped lang="scss">
.container-list {
  display: flex;
  position: relative;
  overflow: hidden;
  width: 100%;
  justify-content: space-between;
  margin: 0 auto;
  padding: 0px 40px;
  background-image: url(../../public/img/footer-bg.jpg);
  background-repeat: no-repeat;
  .container-ul {
    display: flex;
    gap: 50px;
    margin-top: 30px;
    margin-bottom: 30px;

    ul {
      list-style-type: none;

      h2 {
        text-transform: uppercase;
        color: white;
      }

      li {
        margin-top: 10px;
      }

      a {
        text-decoration: none;
        color: gray;
      }

      .shop {
        margin-top: 30px;
      }
    }
  }

  .container-logo {
    position: absolute;
    top: 0;
    right: 0;
    translate: 0 -100px;

    img {
      display: block;
      width: 100%;
      height: 100%;
    }
  }
}
</style>
