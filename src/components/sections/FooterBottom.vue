<template>
  <footer>
    <div class="footer-bottom">
      <div class="container">
        <button>
          <a href="#">sign up now!</a>
        </button>
        <div>
          <h2>follow us</h2>
          <ul>
            <li>
              <a href="">
                <img src="../../assets/img/footer-facebook.png" alt="facebook">
              </a>
            </li>
             <li>
              <a href="">
                <img src="../../assets/img/footer-twitter.png" alt="twitter">
              </a>
            </li>
             <li>
              <a href="">
                <img src="../../assets/img/footer-youtube.png" alt="youtube">
              </a>
            </li>
             <li>
              <a href="">
                <img src="../../assets/img/footer-pinterest.png" alt="pinterest">
              </a>
            </li>
             <li>
              <a href="">
                <img src="../../assets/img/footer-periscope.png" alt="periscope">
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
  name: 'FooterBottom',
  data() {
    return {
      
      

    }
  }
}
</script>

<style scoped lang="scss">
  @import '../../assets/style/partials/variables.scss';
  .footer-bottom {
    background-color: $dc-gray;
    padding: 20px;
  }
  button {
    background: transparent;
    border: 2px solid $dc-blue;
    padding: 10px 10px;
    a {
    text-transform: uppercase;
    text-decoration: none;
    color: white;
    font-weight: bold;
    }

  }
  .container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    > div {
      display: flex;
      align-items: center;
      h2 {
        color: $dc-blue;
        text-transform: uppercase;
        margin-right: 15px;
        font-size: 16px;
      }
      ul {
        display: flex;
        list-style: none;
        img {
          height: 25px;
          margin: 0 5px;
        }
      }
    }
  }



</style>
