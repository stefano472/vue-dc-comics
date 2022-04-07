<template>
  <div class="panel-menu">
    <div class="container">
      <ul class="menu">
        <li>
          <a href="#">
            <img src="@/assets/img/buy-comics-digital-comics.png" alt="digital-comics">
            <span>digital comics</span>
          </a>
        </li>
        <li>
          <a href="#">
            <img src="@/assets/img/buy-comics-merchandise.png" alt="merchandise">
            <span>dc merchandise</span>
          </a>
        </li>
        <li>
          <a href="#">
            <img src="@/assets/img/buy-comics-subscriptions.png" alt="subscription">
            <span>subscription</span>
          </a>
        </li>
        <li>
          <a href="#">
            <img src="@/assets/img/buy-comics-shop-locator.png" alt="shop-locators">
            <span>comic shop locator</span>
          </a>
        </li>
        <li>
          <a href="#">
            <img src="@/assets/img/buy-dc-power-visa.svg" alt="power-visa">
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


<style scoped lang="scss">

.panel-menu {
  background: #0282f9;
}
.menu {
  list-style: none;
  display: flex;
  justify-content: space-around;
  align-items: center;
  padding: 1rem 0;
  li:last-child {
    height: 3.5rem;
    display: flex;
    img {
      height: 1.7rem;
    }
  }
  li {
    border: 0.5rem solid transparent;
    border-radius: 1px;
    &:hover {
      outline: 2px solid white;
    }
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
