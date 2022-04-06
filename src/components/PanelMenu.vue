<template>
  <div class="panel-menu">
    <div class="container">
      <ul class="menu">
        <li>
          <a href="#">
            <img src="../assets/buy-comics-digital-comics.png" alt="digital-comics">
            <span>digital comics</span>
          </a>
        </li>
        <li>
          <a href="#">
            <img src="../assets/buy-comics-merchandise.png" alt="merchandise">
            <span>dc merchandise</span>
          </a>
        </li>
        <li>
          <a href="#">
            <img src="../assets/buy-comics-subscriptions.png" alt="subscription">
            <span>subscription</span>
          </a>
        </li>
        <li>
          <a href="#">
            <img src="../assets/buy-comics-shop-locator.png" alt="shop-locators">
            <span>comic shop locator</span>
          </a>
        </li>
        <li>
          <a href="#">
            <img src="../assets/buy-dc-power-visa.svg" alt="power-visa">
            <span>dc power visa</span>
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'PanelMenu',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.panel-menu {
  background: #0282f9;
}
.menu {
  list-style: none;
  display: flex;
  justify-content: space-around;
  align-items: center;
  padding: 2rem 0;
  li:last-child img {
    height: 1.7rem;
  }
  a {
    color: white;
    text-decoration: none;
    text-transform: uppercase;
    font-size: 0.8rem;
    font-weight: 400;
    display: flex;
    align-items: center;
    gap: 0.8rem;
    img {
      height: 2.5rem;
    }
  }
}
</style>
