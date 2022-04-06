<template>
    <header>
      <div class="container">
        <div class="header-logo">
          <a href="">
            <img src="../assets/dc-logo.png" alt="logo">
          </a>
        </div>
        <nav>
          <ul class="menu">
            <li v-for="link in headerMenu" :key="link" :class="link==='comics'? 'active':''">
              <a href="#"> {{ link }} </a>
            </li>
            <!-- <li>
              <a href="#">character</a>
            </li>
            <li class="active">
              <a href="#">comics</a>
            </li>
            <li>
              <a href="#">movies</a>
            </li>
            <li>
              <a href="#">tv</a>
            </li>
            <li>
              <a href="#">games</a>
            </li>
            <li>
              <a href="#">collectibles</a>
            </li>
            <li>
              <a href="#">videos</a>
            </li>
            <li>
              <a href="#">fans</a>
            </li>
            <li>
              <a href="#">news</a>
            </li>
            <li>
              <a href="#">shop</a>
            </li> -->
          </ul>
        </nav>
      </div>
    </header>
</template>

<script>
export default {
  name: 'HeaderComponents',
  data() {
    return {
      headerMenu: ["character", "comics", "movies", "tv", "games", "collectibles", "videos", "fans", "news", "shop"]
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container {
  display: flex;
  align-items: center;
  justify-content: space-between;
}

img {
  width: 5rem;
}

.menu {
  list-style-type: none;
  display: flex;
  gap: 1rem;
  position: relative;
  
  a{
    color: #2c3e50;
    text-decoration: none;
    text-transform: uppercase;
    font-size: 0.9rem;
    font-weight: 700;
    &:hover {
      color: #0282f9;
    }
  }
}

li {
  position: relative;
  &::before {
    position:absolute;
    content: '';
    bottom: -2.9rem;
    width: 100%;
    height: 4px;
    background: #0282f9;
    transform: scaleY(0);
    transform-origin: bottom;
    transition: transform .3s ease-in-out;
  }
  &:hover::before {
    transform: scaleY(1);
  }
}

.active {
  a {
    color: #0282f9;
  }
  &::before {
    transform: scaleY(1);
  }
}

</style>
