<template>
  <footer>
      <div class="container footer-main clearfix">
          <div class="cols link-cols">
              <div class="list-link">
                  <h3>DC Comics</h3>
                  <ul>
                        <li>
                            <a href="">Characters</a>
                        </li>
                        <li>
                            <a href="">Comics</a>
                        </li>
                        <li>
                            <a href="">Movies</a>
                        </li>
                        <li>
                            <a href="">TV</a>
                        </li>
                        <li>
                            <a href="">Games</a>
                        </li>
                        <li>
                            <a href="">Videos</a>
                        </li>
                        <li>
                            <a href="">News</a>
                        </li>
                  </ul>
                  <h3>Shop</h3>
                  <ul>
                        <li>
                            <a href="">Shop DC</a>
                        </li>
                        <li>
                            <a href="">Shop DC Collectibles</a>
                        </li>
                  </ul>
              </div>
              <div class="list-link">
                  <h3>DC</h3>
                  <ul>
                        <li>
                            <a href="">Terms Of Use</a>
                        </li>
                        <li>
                            <a href="">Privacy policy(New)</a>
                        </li>
                        <li>
                            <a href="">Ad Choices</a>
                        </li>
                        <li>
                            <a href="">Advertising</a>
                        </li>
                        <li>
                            <a href="">Jobs</a>
                        </li>
                        <li>
                            <a href="">Subscriptions</a>
                        </li>
                        <li>
                            <a href="">Talent Workshops</a>
                        </li>
                        <li>
                            <a href="">CPSC Certificatess</a>
                        </li>
                        <li>
                            <a href="">Ratingss</a>
                        </li>
                        <li>
                            <a href="">Shop Helps</a>
                        </li>
                        <li>
                            <a href="">Contact Us</a>
                        </li>
                  </ul>
              </div>
              <div class="list-link">
                  <h3>Sites</h3>
                  <ul>
                        <li>
                            <a href="">DC</a>
                        </li>
                        <li>
                            <a href="">MAD Magazine</a>
                        </li>
                        <li>
                            <a href="">DC Kids</a>
                        </li>
                        <li>
                            <a href="">DC Universe</a>
                        </li>
                        <li>
                            <a href="">DC Power Visa</a>
                        </li>
                  </ul>
              </div>
          </div>
          <div class="cols image"></div>
      </div>
      <div class="footer-bottom">
          <div class="container h-100">
                <button class="btn">SIGN-UP NOW!</button>
                <div class="social">
                    <h3>FOLLOW US</h3>
                    <a href=""><img src="../assets/img/footer-facebook.png" alt=""></a>
                    <a href=""><img src="../assets/img/footer-twitter.png" alt=""></a>
                    <a href=""><img src="../assets/img/footer-youtube.png" alt=""></a>
                    <a href=""><img src="../assets/img/footer-pinterest.png" alt=""></a>
                    <a href=""><img src="../assets/img/footer-periscope.png" alt=""></a>
                </div>
          </div>
      </div>
  </footer>
</template>

<script>
export default {
    name: 'FooterComponent'
}
</script>

<style lang="scss" scoped>
@import "../assets/style/mixins";
@import "../assets/style/vars";


footer{
    height: 400px;
    background-image: url("../assets/img/footer-bg.jpg");

    .container.footer-main{
        height: calc(100% - 80px);
        .cols{
            float: left;
            width: 50%;
            height: 100%;
            &.link-cols{
                padding: 20px 0;
                .list-link{
                    float: left;
                    width: calc(100%/3 - 30px);
                    h3{
                        color: white;
                        padding: 5px 0;
                    }
                    li{
                        padding-top: 5px;
                    }
                    a{
                        color: #70706e;
                        font-size: .9rem;
                    }
                }
            }
            &.image{
                background-image: url("../assets/img/dc-logo-bg.png");
                background-position: center;
                background-size: cover;
            }
        }
    }

    .footer-bottom{
        height: 80px;
        width: 100%;
        background-color: #303030;
        .container{
        @include space-between();
        align-items: center;
        .btn{
            padding: 8px 13px;
            border-radius: 0px;
            border: 1px solid $brand-color;
            background-color: transparent;
            color: white;
            font-weight: bold;
            cursor: pointer;
        }
        .social{
            display: flex;
            align-items: center;
            color: $brand-color;
            img{
                padding: 0 10px;
            }
        }
        }
    }
}

</style>