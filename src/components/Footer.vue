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
        <div class="action">
          <button type="button">SIGN-UP NOW!</button>
        </div>
        <div class="contacts">
          <h2>FOLLOW US</h2>
          <ul class="menu">
            <li>
              <a href="#">
                <img src="../assets/footer-facebook.png" alt="facebook">
              </a>
            </li>
            <li>
              <a href="#">
                <img src="../assets/footer-twitter.png" alt="twitter">
              </a>
            </li>
            <li>
              <a href="#">
                <img src="../assets/footer-youtube.png" alt="youtube">
              </a>
            </li>
            <li>
              <a href="#">
                <img src="../assets/footer-pinterest.png" alt="pinterest">
              </a>
            </li>
            <li>
              <a href="#">
                <img src="../assets/footer-periscope.png" alt="periscope">
              </a>
            </li>
          </ul>       
        </div>
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

  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 1.5rem 0;
  }
}

button {
  padding: 0.6rem;
  background: none;
  color: white;
  font-weight: 600;
  cursor: pointer;
  border: none;
  outline: 2px solid #008dff;
}

.contacts {
  display: flex;
  align-items: center;
  gap: 1rem;
  h2 {
    color: #008dff;
    font-size: 1rem;
  }
  .menu {
    list-style: none;
    display: flex;
    align-items: center;
    gap: 1rem;
    a {
      display: flex;
    }
    img {
      height: 1.8rem;
    }
  }
}
</style>
