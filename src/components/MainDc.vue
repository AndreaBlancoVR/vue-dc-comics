<template>
  <div class="main">
    <div class="container">
      <div class="jumbo-container">
        <div class="jumbo">
        --> Content Goes here --
        </div>
      </div>
      <div class="menu-container">
        <div class="menu-wrapper">
          <ul class="menu">
            <li v-for="(el, i) in MainMenu"  
              class="menu__item"
              :key="i">   
            <figure>
              <img :src="require('../assets/img/' + el.image)">
            </figure>
            <a href="el.href">
              {{ el.text }}
            </a>
            </li>
            <!-- <li class="menu__item">
              <figure>
                <img src="../assets/img/buy-comics-merchandise.png" alt="">
              </figure>
              <a href="" class="">DC Merchandise</a>
            </li>
            <li class="menu__item">
              <figure>
                <img src="../assets/img/buy-comics-subscriptions.png" alt="">
              </figure>
              <a href="" class="">Subscription</a>
            </li>
            <li class="menu__item">
              <figure>
                <img src="../assets/img/buy-comics-shop-locator.png" alt="">
              </figure>
              <a href="" class="">Comic Shop Locator</a>
            </li>
            <li class="menu__item">
              <figure>
                <img src="../assets/img/buy-dc-power-visa.svg" alt="">
              </figure>
              <a href="" class="">DC Power VISA</a>
            </li> -->
          </ul>
        </div>
      </div>
      

  
  
    </div>
  </div>
</template>

<script>
export default {
  name: 'MainDc',
  data() {
    return {
      NavIndex: null,
      MainMenu: [
        {
          text: 'Digital Comics',
          href: '#',
          image: 'buy-comics-digital-comics.png'
        },
        {
          text: 'DC Merchandise',
          href: '#',
          image: 'buy-comics-merchandise.png'
        },
        {
          text: 'Subscription',
          href: '#',
          image: 'buy-comics-subscriptions.png'
        },
        {
          text: 'Comic Shop Locator',
          href: '#',
          image: 'buy-comics-shop-locator.png'
        },
        {
          text: 'DC Power VISA',
          href: '#',
          image: 'buy-dc-power-visa.svg'
        },
        
      ]
    }
  }
}
</script>


<style scoped lang="scss">

  .main {
    justify-content: center;
    display: flex;

    .container {
      width: 100%;
      display: flex;
      flex-direction: column;
      align-items: center;

      .jumbo-container {
        width: 100%;
        display: flex;
        justify-content: center;
        background-color: #1C1C1C;
      }

      .jumbo {
        min-height: 132px;
        width: 1280px;
        
        color: white;
      }

      .menu-container {
        width: 100%;
        display: flex;
        justify-content: center;
        background-color: #0282F9;
      }
      .menu-wrapper{
        display: flex;
        justify-content: center;
        width: 1280px;
        height: 155px;

      }
      .menu {
          display: flex;
          width: 100%;
          justify-content: space-between;
          padding: 0 14px;
          gap: 74px;
          padding: 0 36px;

          .menu__item {
            display: flex;
            align-items: center;

            figure {
              display: flex;
              width: 55px;
              height: 55px;
              margin: 0;
              padding-right: 11px;
              cursor: pointer;
            }

            a {
            text-decoration: none;
            color: white;
            font-size: 12px;
            font-weight: 700;
            text-transform: uppercase;
            }
          }
      }
    }
  }
</style>
