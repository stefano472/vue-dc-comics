<template>
  <footer>
    <div class="hero-footer container">
      <div class="footer-comics-nav">
        <h2>DC COMICS</h2>
        <ul>
          <li>
            <a href="#">Characters</a>
          </li>
          <li>
            <a href="#">Comics</a>
          </li>
          <li>
            <a href="#">Movies</a>
          </li>
          <li>
            <a href="#">TV</a>
          </li>
          <li>
            <a href="#">Games</a>
          </li>
          <li>
            <a href="#">Videos</a>
          </li>
          <li>
            <a href="#">News</a>
          </li>
        </ul>
        <h2>SHOP</h2>
        <ul>
          <li>
            <a href="#">Shop DC</a>
          </li>
          <li>
            <a href="#">Shop DC Collectibles</a>
          </li>
        </ul>
      </div>

      <div class="footer-DC-nav">
        <h2>DC</h2>
        <ul>
          <li>
            <a href="#">Characters</a>
          </li>
          <li>
            <a href="#">Comics</a>
          </li>
          <li>
            <a href="#">Movies</a>
          </li>
          <li>
            <a href="#">TV</a>
          </li>
          <li>
            <a href="#">Games</a>
          </li>
          <li>
            <a href="#">Videos</a>
          </li>
          <li>
            <a href="#">News</a>
          </li>
        </ul>
      </div>

      <div class="footer-site-nav">
        <h2>SITES</h2>
        <ul>
          <li>
            <a href="#">Characters</a>
          </li>
          <li>
            <a href="#">Comics</a>
          </li>
          <li>
            <a href="#">Movies</a>
          </li>
          <li>
            <a href="#">TV</a>
          </li>
          <li>
            <a href="#">Games</a>
          </li>
          <li>
            <a href="#">Videos</a>
          </li>
          <li>
            <a href="#">News</a>
          </li>
        </ul>
      </div>
    </div>

    <div class="bottom-footer">
      <div class="container">
        <h2>sign up now</h2>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'FooterComponents',
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
footer {
  background-image: url("../assets/footer-bg.jpg");
  background-size: cover;
  background-repeat: no-repeat;
}
.hero-footer {
  padding: 1rem 0;
  display: flex;
  gap: 1.5rem;
  background-image: url("../assets/dc-logo-bg.png");
  background-repeat: no-repeat;
  background-position: center right;
  background-size: 50%;
  &>div{
    padding-bottom: 1.5rem;
  }
  h2 {
    color: white;
    font-size: 1rem;
    font-weight: 500;
    padding: 0.8rem 0;
  }
  ul {
    list-style: none;
    a {
      color: #999;
      text-decoration: none;
      font-size: 0.8rem;
    }
  }
}
.bottom-footer {
  background: #303030;
  color: white;
}
</style>
