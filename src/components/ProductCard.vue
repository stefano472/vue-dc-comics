<template>
  <div class="card">
      <img :src="img" :alt="title">
      <div class="definition">
        <h5>{{ type }}</h5>
        <h2>{{ title }}</h2>
        <p>Price: {{ price }}</p>
      </div>
  </div>
</template>

<script>
export default {
    name: 'ProductCard',
    props: {
        img: String,
        price: String,
        title: String,
        type: String
    }
}
</script>

<style lang="scss" scoped>
.card {
    flex-basis: calc(100% / 6 - 0.8rem * 5 / 6);
    position: relative;
    display: flex;
    flex-direction: column;
    &:hover {
        h2 {
            color: #0075f9;
        }
        img {
            opacity: 0.6;
            // aspect-ratio: auto;
        }
    }
}
img {
    width: 100%;
    // aspect-ratio: 1/1;
    // object-fit: cover;
    // object-position: top;
}
h5 {
    padding-top: 0.6rem;
    font-size: 0.8rem;
    text-transform: uppercase;
    color: #0075f9;
    font-weight: 700;

}
h2 {
    text-transform: uppercase;
    word-break: break-word;
    font-size: 1.2rem;
    padding: 0.3rem 0;
}
p {
    font-size: 0.9rem;
    color: #66e06b;
    font-weight: 700;
    text-transform: uppercase;
}
</style>