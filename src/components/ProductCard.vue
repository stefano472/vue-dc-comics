<template>
  <div class="card">
      <img :src="img" :alt="title">
      <h5>{{ type }}</h5>
      <h2>{{ title }}</h2>
      <p>Price: {{ price }}</p>
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
    display: flex;
    flex-direction: column;
    &:hover {
        h2 {
            color: #0075f9;
        }
        img {
            opacity: 0.5;
        }
    }
}
img {
    width: 100%;
    // height: 8rem;
    // object-fit: cover;
    // object-position: top;
}
h5 {
    padding-top: 0.5rem;
    font-size: 0.8rem;
    text-transform: uppercase;
    color: #0075f9;
    font-weight: 700;

}
h2 {
    text-transform: uppercase;
    word-break: break-word;
    font-size: 1.3rem;
}
p {
    font-size: 0.9rem;
    color: #66e06b;
    font-weight: 700;
    text-transform: uppercase;
}
</style>