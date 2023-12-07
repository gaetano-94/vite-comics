<script>
export default {
  name: 'Navbar',
  data() {
    return {
      navbar: [
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
          nome: 'Collectubles',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Videos',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Fans',
          link: '#',
          target: '_self',
        },
        {
          nome: 'News',
          link: '#',
          target: '_self',
        },
        {
          nome: 'Shop',
          link: '#',
          target: '_self',
        },
      ],
    };
  },
};
</script>

<template>
  <ul class="menu">
    <li v-for="li in navbar" class="list">
      <a :href="li.link" :target="li.target">{{ li.nome }}</a>
    </li>
  </ul>
</template>

<style scoped lang="scss">
@use '../styles/partials/variables..scss' as *;
.menu {
  display: flex;
  list-style-type: none;
  gap: 20px;

  a {
    color: black;
    text-decoration: none;
    text-transform: uppercase;
    &:hover {
      color: $secondary;
    }
  }
}
</style>
