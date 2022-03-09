<template>
              <li class="card-wrapper">
                <figure class="card-header">
                    <div class="overlay">
                        <p>
                            {{ price }}
                        </p>

                    </div>
                  <img :src="thumb" alt="">
                </figure>
                <h3 class="card-footer">
                  {{ series }}
                </h3>
              </li>
</template>

<script>
    export default {
        props: ['thumb', 'price', 'series', 'type'],
    }

</script>

<style lang="scss" scoped>
    .card-wrapper {
        display: flex;
        flex-direction: column;
        width: calc(95% / 6);
        min-width: 150px;
        // height: 240px;
        padding: 8px;
        cursor: pointer;

      }

      .card-header {
        display: flex;
        position: relative;
        // width: 185px;
        // height: 185px;
        width: 100%;
        aspect-ratio: 1;

        img {
              display: flex;
              width: 100%;
              object-fit: cover;
              object-position: top;
        }
      }

      .card-footer {
        width: 100%;
        height: 55px;
        padding: 23px 0;
        text-transform: uppercase;
        font-size: 12px;
      }

      .overlay {
          background-color: #0282F9;
          position: absolute;
          width: 100%;
          height: 100%;
          display: none;
          color: white;
          font-size: 30px;
          text-align: center;
          cursor: pointer;

          p {
              z-index: 999;
              top: 50%;
              left: 50%;
              transform: translate(-50%, -50%);
              position: absolute; 
          }
      }

      .card-header:hover .overlay{
          display: block;
      }

    //   .active {
    //       display: block;
    //   }
</style>
