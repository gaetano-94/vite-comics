<script>
export default {
  name: 'MainBottom',
  data() {
    return {
      cardHeroes: [
        {
          thumb: 'https://www.coverbrowser.com/image/action-comics/1-1.jpg',
          price: '$19.99',
          series: 'Action Comics',
          type: 'comic book',
        },
        {
          thumb:
            'https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg',
          price: '$3.99',
          series: 'American Vampire 1976',
          type: 'comic book',
        },
        {
          thumb:
            'https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg',
          price: '$16.99',
          series: 'Aquaman',
          type: 'graphic novel',
        },
        {
          thumb: 'https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg',
          price: '$2.99',
          series: 'Batgirl',
          type: 'comic book',
        },
        {
          thumb:
            'https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg',
          price: '$3.99',
          series: 'Batman',
          type: 'comic book',
        },
        {
          thumb:
            'https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg',
          price: '$2.99',
          series: 'Batman Beyond',
          type: 'comic book',
        },
        {
          thumb:
            'https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg',
          price: '$3.99',
          series: 'Batman/Superman',
          type: 'comic book',
        },
        {
          thumb:
            'https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg',
          price: '$4.99',
          series: 'Batman/Superman Annual',
          type: 'comic book',
        },
        {
          thumb:
            'https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg',
          price: '$5.99',
          series: 'Batman: The Joker War Zone',
          type: 'comic book',
        },
        {
          thumb:
            'https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg',
          price: '$6.99',
          series: 'Batman: Three Jokers',
          type: 'comic book',
        },
        {
          thumb:
            'https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg',
          price: '$4.99',
          series: 'Batman: White Knight Presents: Harley Quinn',
          type: 'comic book',
        },
        {
          thumb:
            'https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg',
          price: '$16.99',
          series: 'Catwoman',
          type: 'graphic novel',
        },
      ],
    };
  },
};
</script>

<template>
  <section>
    <button class="button-top"><strong>Current Series</strong></button>
    <div class="container">
      <div class="heroes">
        <div class="hero" v-for="hero in cardHeroes">
          <figure>
            <img :src="hero.thumb" :alt="hero.series" />
          </figure>
          <h4>{{ hero.series }}</h4>
        </div>
        <button class="button-bottom">Load More</button>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
@use '../styles/partials/variables..scss' as *;
section {
  width: 100%;
  background-color: $black;
  padding: 50px 0px 0px 0px;
  position: relative;

  .button-top {
    position: absolute;
    top: 0;
    margin: 0px auto;
    padding: 10px 30px 10px 30px;
    text-transform: uppercase;
    cursor: pointer;
    background-color: $primary;
    border: none;
    color: white;
    font-size: 20px;
    margin-left: 40px;
  }

  .container {
    max-width: 1250px;
    margin: auto;

    .heroes {
      display: flex;
      flex-wrap: wrap;

      .hero {
        width: calc(100% / 6);
        border: 10px solid $black;

        h4 {
          color: white;
          margin-top: 15px;
        }

        figure {
          height: 200px;
        }
        img {
          width: 100%;
          height: 100%;
          object-fit: cover;
          object-position: top;
        }
      }

      .button-bottom {
        margin: 20px auto;
        padding: 10px 50px 10px 50px;
        text-transform: uppercase;
        cursor: pointer;
        background-color: $primary;
        border: none;
        color: white;
      }
    }
  }
}
</style>
