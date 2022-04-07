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

<style>
img {
    transform: scale(0.9);
}
h5 {
    font-size: 0.8rem;
    text-transform: uppercase;
    color: #0075f9;
    font-weight: 700;

}
h2 {
    text-transform: uppercase;
}
p {
    color: #66e06b;
    font-weight: 700;
    text-transform: uppercase;

}
</style>