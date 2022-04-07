<template>
  <main>
    <div class="hero">
        <div class="container">
          <div class="active-series">
            CURRENT SERIES
          </div>
        </div>
    </div>
    <div class="container">
      <div class="contents">
        <ProductCard v-for="card in dcComics" :key="card.series" :img="card.thumb" :price="card.price" :title="card.series" :type="card.type"/>
      </div>
      <div class="more">
        <button type="button">LOAD MORE</button>
      </div>
    </div>
  </main>
</template>

<script>

import dcComics from '@/assets/data/dc-comics'
import ProductCard from '@/components/ProductCard'

export default {
  name: 'MainComponents',
  data() {
    return {
      dcComics,
    }
  }, 
  components: {
    ProductCard,
  }
}
</script>

<style scoped lang="scss">

main {
  color: white;
  background: #1c1c1c;
  .hero {
    height: 20rem;
    background-image: url("@/assets/img/jumbotron.jpg");
    background-position: top center;
    background-size: cover;
    position: relative;
    .active-series {
      position: absolute;
      transform: translateY(50%);
      bottom: 0;
      font-size: 0.9rem;
      font-weight: 700;
      padding: 0.5rem 1rem;
      border-radius: 1px;
      background-color: #0282f9;
    }
  }
  .contents {
    display: flex;
    flex-wrap: wrap;
    gap: 0.8rem;
    padding: 1.5rem 0;
    // ProductCard {
    //   flex-basis: calc(100% / 6 - 0.8rem * 5 / 6);
    //   display: flex;
    //   flex-direction: column;
    // }
  }
  .more {
    padding: 1rem 0;
    text-align: center;
    button {
      border: none;
      border-radius: 1px;
      color: white;
      font-size: 0.8rem;
      font-weight: 700;
      padding:  0.5rem 1.5rem;
      background: #0282f9;
      transition: 0.3s;
      cursor: pointer;
      &:hover {
          box-shadow: inset 0px 0px 0 2px;
          border-radius: 5px;
      }
    }
  }
}

</style>
