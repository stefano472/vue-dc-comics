<template>
    <header>
      <div class="container">
        <div class="logo">
          <img src="../assets/dc-logo.png" alt="logo">
        </div>
        <nav>
          <ul class="menu">
            <li>
              <a href="#">character</a>
            </li>
            <li>
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
            </li>
          </ul>
        </nav>
      </div>
    </header>
</template>

<script>
export default {
  name: 'HeaderComponents',
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
  a{
    color: #2c3e50;
    text-decoration: none;
    text-transform: uppercase;
    font-size: 0.9rem;
    font-weight: 700;
  }
}
</style>
