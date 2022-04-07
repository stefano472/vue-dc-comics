<template>
    <header>
      <div class="container">
        <div class="header-logo">
          <a href="">
            <img src="@/assets/img/dc-logo.png" alt="logo">
          </a>
        </div>
        <nav>
          <ul class="menu">
            <li v-for="link in headerMenu" :key="link.name" :class="link.active? 'active':''">
              <a href="#"> {{ link.name }} </a>
            </li>
       
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
      headerMenu: [
        {
          name: 'character',
          active: false
        }, 
        {
          name: 'comics',
          active: true
        }, 
        {
          name: 'movies',
          active: false
        }, 
        {
          name: 'tv',
          active: false
        }, 
        {
          name: 'games',
          active: false
        }, 
        {
          name: 'collectibles',
          active: false
        }, 
        {
          name: 'videos',
          active: false
        }, 
        {
          name: 'fans',
          active: false
        }, 
        {
          name: 'news',
          active: false
        }, 
        {
          name: 'shop',
          active: false
        }
      ]
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
  gap: 0.5rem;
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
