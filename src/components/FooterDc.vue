<template>
  <div class="footer">
    <div class="container">
      <div class="footer_up">
        <section class="footer_up-left">
          <div class="ul-1-2">
            <h2 class="map-title">DC Comics</h2>
            <div class="">
              <ul class="menu">
                <li v-for="(el, i) in UlOne" 
                class="menu__item" 
                :key="i">
                  <a href="el.href">{{ el.text }}</a>
                </li>
                <!-- <li class="menu__item">
                  <a href="">Comics</a
                ></li>
                <li class="menu__item">
                  <a href="">Movies</a>
                </li>
                <li class="menu__item">
                  <a href="">TV</a>
                </li>
                <li class="menu__item">
                  <a href="">Games</a>
                </li>
                <li class="menu__item">
                  <a href="">Videos</a>
                </li>
                <li class="menu__item">
                  <a href="">News</a>
                </li>
                <li class="menu__item">
                  <a href="">DC Shop</a>
                </li> -->
              </ul>    
            </div>
            <h2 class="">Shop</h2>
            <div class="">
              <ul class="menu">
                <li v-for="(el, i) in UlTwo"
                class="menu__item"
                :key="i">
                  <a href="el.href">{{ el.text }}</a>
                </li>
                <!-- <li class="menu__item">
                  <a href="">Shop DC Collectibles</a>
                </li> -->
              </ul>
            </div>
          </div>
          <div class="">
            <h2 class="">DC</h2>
            <div class="">
              <ul class="menu">
                <li v-for="(el, i) in UlThree" 
                class="menu__item"
                :key="i">
                  <a href="el.href">{{ el.text}}</a>
                </li>
                <!-- <li class="menu__item">
                  <a href="">Privacy Policy (New)</a>
                </li>
                <li class="menu__item">
                  <a href="">Ad Choices</a>
                </li>
                <li class="menu__item">
                  <a href="">Advertising</a>
                </li>
                <li class="menu__item">
                  <a href="">Jobs</a>
                </li>
                <li class="menu__item">
                  <a href="">Subscriptions</a>
                </li>
                <li class="menu__item">
                  <a href="">CPSC Certificates</a>
                </li>
                <li class="menu__item">
                  <a href="">Ratings</a>
                </li>
                <li class="menu__item">
                  <a href="">Shop Help</a>
                </li>
                <li class="menu__item">
                  <a href="">Contact Us</a>
                </li> -->
              </ul>    
            </div>
          </div>
          <div class="">
            <h2 class="">Sites</h2>
            <div class="">
              <ul class="menu">
                <li v-for="(el, i) in UlFour"
                class="menu__item"
                :key="i">
                  <a href="el.href">{{ el.text }}</a>
                </li>
                <!-- <li class="menu__item">
                  <a href="">DC Power Visa</a>
                </li>
                <li class="menu__item">
                  <a href="">DC Kids</a>
                </li>
                <li class="menu__item">
                  <a href="">DC Universe</a>
                </li>
                <li class="menu__item">
                  <a href="">MAD Magazine</a>
                </li> -->
              </ul>    
            </div>
          </div>
        </section> 
        <section class="footer_up-right">
          <div class="">
          </div>
        </section> 
      </div>
      <div class="footer_down">
        <div class="footer_down-wrapper">
              <div class="sign-up">
                <p>
                  <a href="">Sign-Up Now!</a>
                </p>    
              </div>
            <div class="social-wrapper">
              <h2 class="">Follow us</h2>
              <div class="social-items">
                <ul class="menu">
                  <li v-for="(el, i) in UlIcons" 
                  class=""
                  :key="i">
                    <a href="">
                      <img :src="require('../assets/img/' + el.icon)">
                    </a>
                    
                  </li>
                  <!-- <li class=""><img src="../assets/img/footer-twitter.png" alt=""></li>
                  <li class=""><img src="../assets/img/footer-youtube.png" alt=""></li>
                  <li class=""><img src="../assets/img/footer-pinterest.png" alt=""></li>
                  <li class=""><img src="../assets/img/footer-periscope.png" alt=""></li> -->
                </ul>    
              </div>
            </div>
        </div>
      </div> 
    </div>         
  </div>
</template>

<script>
export default {
  name: 'FooterDc',
  data() {
    return {
      UlOne: [
        {
          text: 'Characters',
          href: '#',
        },
        {
          text: 'Comics',
          href: '#',
        },
        {
          text: 'Movies',
          href: '#',
        },
        {
          text: 'TV',
          href: '#',
        },
        {
          text: 'Games',
          href: '#',
        },
        {
          text: 'Videos',
          href: '#',
        },
        {
          text: 'News',
          href: '#',
        },
        {
          text: 'DC Shop',
          href: '#',
        },        
      ],

      UlTwo: [
        {
          text: 'Shop DC',
          href: '#',
        },
        {
          text: 'Shop DC Collectibles',
          href: '#',
        },
      ],
      UlThree: [
        {
          text: 'Terms of Use',
          href: '#',
        },
        {
          text: 'Privacy Policy (New)',
          href: '#',
        },
        {
          text: 'Ad Choices',
          href: '#',
        },
        {
          text: 'Advertising',
          href: '#',
        },
        {
          text: 'Jobs',
          href: '#',
        },
        {
          text: 'Subscriptions',
          href: '#',
        },
        {
          text: 'CPSC Certificates',
          href: '#',
        },
        {
          text: 'Ratings',
          href: '#',
        },
        {
          text: 'Shop Help',
          href: '#',
        },  
        {
          text: 'Contact Us',
          href: '#',
        },          
      ],

      UlFour: [
        {
          text: 'DC',
          href: '#',
        },
        {
          text: 'MAD Magazine',
          href: '#',
        },
        {
          text: 'DC Kids',
          href: '#',
        },
        {
          text: 'DC Universe',
          href: '#',
        },
        {
          text: 'DC Power Visa',
          href: '#',
        },
      ],

      UlIcons: [
        {
          icon: 'footer-facebook.png',
        },
        {
          icon: 'footer-twitter.png',
        },
        {
          icon: 'footer-youtube.png',
        },
        {
          icon: 'footer-pinterest.png',
        },
        {
          icon: 'footer-periscope.png',
        },
      ],
    }
  }
}
</script>


<style scoped lang="scss">
  .footer {
    justify-content: center;
    display: flex;

    .container {
      width: 100%;
      display: flex;
      flex-direction: column;
      justify-content: center;
      align-items: center;
      background-image: url("../assets/img/footer-bg.jpg");
      background-repeat: no-repeat;
      background-size: 100%;

      .footer_up {
        width: 1280px;
        height: 370px;
        
        display: flex;

        .footer_up-left {
          width: 50%;
          display: flex;
          justify-content: flex-start;
          padding-top: 30px;
          gap: 25px;

          h2 {
            color: white;
            text-transform: uppercase;
          }

          .menu {
            padding: 0;
            .menu__item {
              

              a {
              text-decoration: none;
              color: #959595;
              font-size: 12px;
              font-weight: 700;
              
              }
            }
          }
        }

        .footer_up-right {
          width: 50%;
          background-image: url("../assets/img/dc-logo-bg.png");
          background-position: center;
          background-repeat: no-repeat;
        }

        
      }
      .footer_down {
        width: 100%;
        height: 110px;
        display: flex;
        justify-content: center;
        background-color: #303030;

        .footer_down-wrapper {
          width: 1280px;
          display: flex;
          justify-content: space-between;
          align-items: center;
        }

        .sign-up {

          a {
            text-decoration: none;
            color: white;
            font-size: 12px;
            font-weight: 700;
            text-transform: uppercase;
            border: 2px solid #0282F9;
            padding: 17px 15px
          }
        }

        .social-wrapper {
          display: flex;
          align-items: center;
          gap: 30px;
          color: #0282F9;
          text-transform: uppercase;

          ul {
            display: contents;

            a {
              display: contents;
            }
          }
        }

        .social-items {
          display: flex;
          gap: 19px;
        }
      }
    }
  }

</style>