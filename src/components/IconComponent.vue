<template>
  <div id="icon-box">
      <div class="h-100 container">
          <ul class="h-100">
            <li>
                <img src="../assets/img/buy-comics-digital-comics.png" alt="Digital Comics">
                <a href="#">Digital Comics</a>
            </li>
            <li>
                <img src="../assets/img/buy-comics-merchandise.png" alt="Digital Comics">
                <a href="#">DC Merchandise</a>
            </li>
            <li>
                <img src="../assets/img/buy-comics-subscriptions.png" alt="Digital Comics">
                <a href="#">Subscription</a>
            </li>
            <li>
                <img src="../assets/img/buy-comics-shop-locator.png" alt="Digital Comics">
                <a href="#">Comic Shop Locator</a>
            </li>
            <li>
                <img src="../assets/img/buy-dc-power-visa.svg" alt="Digital Comics">
                <a href="#">DC Power visas</a>
            </li>
          </ul>
      </div>
  </div>
</template>

<script>
export default {
    name: 'IconComponent',
}
</script>

<style lang="scss" scoped>

@import "../assets/style/vars";

#icon-box{
    height: 120px;
    background-color: $brand-color;
    ul{
        display: flex;
        align-items: center;
        li{
            display: flex;
            align-items: center;
            flex-basis: calc(100% / 5);
            height: 50%;
            padding: 0 20px;
        }
        img{
        height: 45px;
        max-width: 40px;
        }
        a{
        font-size: .9rem;
        margin-left: 15px;    
        text-transform: uppercase;
        color: white;
        }
    }
    
}

</style>