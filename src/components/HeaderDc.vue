<template>
  <div class="header">
    <div class="container-fluid">
      <div class="container">
        <figure class="logo">
          <img src="../assets/img/dc-logo.png" alt="">
      </figure>
      <nav class="main-nav nav">
        <ul>
          <li v-for="(el, i) in HeaderMenu" 
            :class=" NavIndex == i ? 'active' : '' " 
            class="nav__item"
            @mouseenter="NavIndex = i"
            @mouseleave="NavIndex = null" 
            :key="i">   
            <a :href="el.href">
              {{ el.text }}
            </a>
          </li> 
          <!-- <li class="nav__item">
            <a href="">
              Character
            </a>
          </li>
          <li class="nav__item active">
            <a href="">
              Comics
            </a>
          </li>
          <li class="nav__item">
            <a href="">
              Movies
            </a>
          </li>
          <li class="nav__item">
            <a href="">
              TV
            </a>
          </li>
          <li class="nav__item">
            <a href="">
              Games
            </a>
          </li>
          <li class="nav__item">
            <a href="">
              Collectibles
            </a>
          </li>
          <li class="nav__item">
            <a href="">
              Videos
            </a>
          </li>
          <li class="nav__item">
            <a href="">
              Fans
            </a>
          </li>
          <li class="nav__item">
            <a href="">
              News
            </a>
          </li>
          <li class="nav__item">
            <a href="">
              Shop
            </a>
          </li> -->
        </ul>
      </nav>
      </div>
      
    </div>
  </div>
</template>

<script>
export default {
  name: 'HeaderDc',
  data() {
    return {
      NavIndex: null,
      HeaderMenu: [
        {
          text: 'Character',
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
          text: 'Collectibles',
          href: '#',
        },
        {
          text: 'Videos',
          href: '#',
        },
        {
          text: 'Fans',
          href: '#',
        },
        {
          text: 'News',
          href: '#',
        },
        {
          text: 'Shop',
          href: '#',
        },
      ]
    }
  }
  // methods() {
  //   return {
  //     NavIndexFn: function( i ){
  //           this.NavIndex = i
  //       },
  //   }
  // }
}
</script>


<style scoped lang="scss">
.header {
    height: 118px;
    justify-content: center;
    display: flex;

    .container-fluid {
    width: 100%;
    display: flex;
    justify-content: center;
    }

    .container {
      width: 1280px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .logo {
      display: flex;
      width: 80px;
      height: 80px;
      margin: 0;
      cursor: pointer;
    }

    .main-nav {
      display: flex;
      justify-content: center;

      ul {
        display: flex;
        padding: 0 14px;
        gap: 34px;
      }

      .nav__item {
        a {
          text-decoration: none;
          color: currentColor;
          font-size: 12px;
          font-weight: 700;
          text-transform: uppercase;
        }

        &.active {
          color: #0282F9;
          position: relative;
        }

        &.active::after {
          content: '';
          display: block;
          height: 5px;
          width: 100%;
          background-color: #0282F9;
          position: absolute;
          top: 63px;
          left: 50%;
          transform: translateX(-50%);
        }
      }
    }
}
</style>
