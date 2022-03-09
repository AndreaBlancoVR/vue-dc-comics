<template>
  <div class="main">
    <div class="container">
      <div class="jumbo-up-container">
        <div class="jumbo-up">
          <a href="">
            Current series
          </a>
        </div>
      </div>
      <div class="jumbo-container">
        <div class="jumbo">
          <div class="row">
            <ul>
              <ComicsDc v-for="(el, i) in CardsData" :key="i" :thumb="el.thumb" :series="el.series" />
            </ul>
            
            <!-- <ul>
              <li class="card-wrapper">
                <figure class="card-header">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
                </figure>
                <h3 class="card-footer">
                  Action Comics
                </h3>
              </li>
              <li class="card-wrapper">
                <figure class="card-header">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
                </figure>
                <h3 class="card-footer">
                  Action Comics
                </h3>
              </li>
              <li class="card-wrapper">
                <figure class="card-header">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
                </figure>
                <h3 class="card-footer">
                  Action Comics
                </h3>
              </li>
              <li class="card-wrapper">
                <figure class="card-header">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
                </figure>
                <h3 class="card-footer">
                  Action Comics
                </h3>
              </li>
              <li class="card-wrapper">
                <figure class="card-header">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
                </figure>
                <h3 class="card-footer">
                  Action Comics
                </h3>
              </li>
              <li class="card-wrapper">
                <figure class="card-header">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
                </figure>
                <h3 class="card-footer">
                  Action Comics
                </h3>
              </li>
              <li class="card-wrapper">
                <figure class="card-header">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
                </figure>
                <h3 class="card-footer">
                  Action Comics
                </h3>
              </li>
              <li class="card-wrapper">
                <figure class="card-header">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
                </figure>
                <h3 class="card-footer">
                  Action Comics
                </h3>
              </li>
              <li class="card-wrapper">
                <figure class="card-header">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
                </figure>
                <h3 class="card-footer">
                  Action Comics
                </h3>
              </li>
              <li class="card-wrapper">
                <figure class="card-header">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
                </figure>
                <h3 class="card-footer">
                  Action Comics
                </h3>
              </li>
              <li class="card-wrapper">
                <figure class="card-header">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
                </figure>
                <h3 class="card-footer">
                  Action Comics
                </h3>
              </li>
              <li class="card-wrapper">
                <figure class="card-header">
                  <img src="https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX" alt="">
                </figure>
                <h3 class="card-footer">
                  Action Comics
                </h3>
              </li>
            </ul> -->
            
          </div>
          <div class="row_2">
              <a href="">
                Load more
              </a>
          </div>
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
// import ComicsDc from '.ComicsDc.vue'
import ComicsDc from './ComicsDc.vue'


export default {
  components: { ComicsDc },
  name: 'MainDc',
  data() {
    return {
      NavIndex: null,
      CardsData: [
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/AC1000_DLX_162-001_HD_5ba13723281ab0.37845353.jpg?itok=ZsI-C5eX",
          "price": "$19.99",
          "series": "Action Comics",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/AV1976_01_300-001_HD_5f738f6e39ddd7.18205602.jpg?itok=VgdYdJ01",
          "price": "$3.99",
          "series": "American Vampire 1976",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2018/08/AQMv4_UW_153-001_HD_5b7efa1745a9b8.08589135.jpg?itok=HPTtnrsb",
          "price": "$16.99",
          "series": "Aquaman",
          "type": "graphic novel"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/06/batgirl_v5_1_5b23e1f1124941.50950783.jpg?itok=VnrJah76",
          "price": "$2.99",
          "series": "Batgirl",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          "price": "$3.99",
          "series": "Batman",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2018/09/BM_56_300-001_HD_5ba137a85c3bf3.33122291.jpg?itok=3FHJQYJZ",
          "price": "$2.99",
          "series": "Batman Beyond",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2019/08/BMSM_5d4361b7116261.74371456.jpg?itok=kEDR2OL8",
          "price": "$3.99",
          "series": "Batman/Superman",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMSMANN_01_300-001_HD_5f5ff17fa1d665.74704970.jpg?itok=azz5sfGk",
          "price": "$4.99",
          "series": "Batman/Superman Annual",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/09/BMTJWZ_01_300-001_HD_5f5ff2307dcb37.34652945.jpg?itok=VswVjLR8",
          "price": "$5.99",
          "series": "Batman: The Joker War Zone",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/08/cover-v2_5f40314645a734.37285065.png?itok=ImNM2QBY",
          "price": "$6.99",
          "series": "Batman: Three Jokers",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/comic-covers/2020/10/BMWK_HQ_01_300-001_HD_5f7cb4945e13f6.89501032.jpg?itok=sVwALbUX",
          "price": "$4.99",
          "series": "Batman: White Knight Presents: Harley Quinn",
          "type": "comic book"
        },
        {
          "thumb": "https://www.dccomics.com/sites/default/files/styles/covers192x291/public/gn-covers/2019/04/CTWv1_CC_144-001_HD_5ca5299a751963.53054221.jpg?itok=ooPaoLDq",
          "price": "$16.99",
          "series": "Catwoman",
          "type": "graphic novel"
        }
      ],

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
        // min-height: 668px;
      }

      .jumbo-up-container {
        width: 100%;
        height: 400px;
        background-image: url("../assets/img/jumbotron.jpg");
        // background-size: 100%;
        background-repeat: no-repeat;
        display: flex;
        justify-content: center;

        .jumbo-up {
          position: relative;
          width: 100%;
          max-width: 1280px;
          

          a {
            text-decoration: none;
            color: white;
            font-size: 12px;
            font-weight: 700;
            text-transform: uppercase;
            background-color: #0282F9;
            padding: 10px 55px;
            position: absolute;
            white-space: nowrap;
            bottom: -16px;
            left: 0px;
          }
        }
      }

      .jumbo {
        min-height: 132px;
        width: 1280px;
        color: white;
      }

      .row {
        display: flex;
        flex-basis: 100%;
        gap: 1%;
        justify-content: space-between;
        flex-wrap: wrap;
        padding: 52px 14px;

        ul {
          display: contents;
        }
      }

      // .card-wrapper {
      //   display: flex;
      //   flex-direction: column;
      //   width: calc(95% / 6);
      //   height: 240px;

      // }

      // .card-header {
      //   display: flex;
      //   position: relative;
      //   width: 185px;
      //   height: 185px;

      //   img {
      //         display: flex;
      //         width: 100%;
      //         object-fit: cover;
      //         object-position: top;
      //   }
      // }

      // .card-footer {
      //   width: 100%;
      //   height: 55px;
      //   line-height: 55px;
      //   text-transform: uppercase;
      //   font-size: 14px;
      // }

      .row_2 {
        display: flex;
        justify-content: center;
        margin-bottom: 20px;
        a {
          text-decoration: none;
          color: white;
          font-size: 12px;
          font-weight: 700;
          text-transform: uppercase;
          background-color: #0282F9;
          padding: 10px 55px
        }
      }

      .menu-container {
        width: 100%;
        display: flex;
        justify-content: center;
        background-color: #0282F9;
      }

      .menu-wrapper {
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
