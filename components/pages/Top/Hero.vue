<template>
  <div class="home-Title">
    <div class="st-Container">
      <div class="home-Title_Cloud1"></div>
      <div class="home-Title_Cloud2"></div>
      <div class="home-Title_Logo"></div>
    </div>
    <div class="home-Title_Cloud3"></div>
    <div class="home-Title_Cloud4"></div>
    <div class="home-Title_Wave"></div>
    <div class="home-Title_Elephants">
      <a class="home-Title_Attention" href="#home-Wanted">スポンサー募集中！</a>
      <div class="home-Title_Elephant"></div>
    </div>
  </div>
</template>

<script>
</script>

<style lang="scss" scoped>
  @import "~assets/scss/library/_variable.scss";
  @import "~assets/scss/library/_mixin.scss";

  .home-Title {
    width: auto;
    background-color: $clr_main;
    position: relative;
    .st-Container {
      height: 750px;
      position: relative;
      .home-Title_Cloud1 {
        margin-left: 100px;
        width: 200px;
        height: 132px;
        background-image: url("/images/aerialCloud.png");
        background-repeat: no-repeat;
        background-size: contain;
        position: absolute;
        top: 450px;
        left: 0;
      }
      .home-Title_Cloud2 {
        margin-right: 130px;
        width: 180px;
        height: 122px;
        background-image: url("/images/airplane.png");
        background-repeat: no-repeat;
        background-size: contain;
        position: absolute;
        top: 150px;
        right: 0;
      }
      .home-Title_Logo {
        z-index: 100;
        margin-left: auto;
        margin-right: auto;
        width: 323px;
        height: 542px;
        background-image: url("/images/title.svg");
        background-repeat: no-repeat;
        position: absolute;
        top: 50px;
        left: 0;
        right: 0;
        bottom: 0;
      }
    }
    .home-Title_Cloud3 {
      z-index: 1;
      width: 399px;
      height: 555px;
      background-image: url("/images/cloud_left.png");
      background-repeat: no-repeat;
      background-size: contain;
      position: absolute;
      top: 210px;
      left: 0;
    }
    .home-Title_Cloud4 {
      z-index: 1;
      width: 399px;
      height: 555px;
      background-image: url("/images/cloud_right.png");
      background-repeat: no-repeat;
      background-size: contain;
      position: absolute;
      top: 180px;
      right: 0;
    }
    .home-Title_Wave {
      z-index: 2;
      width: 100%;
      height: 217px;
      background-image: url("/images/ocean.png");
      background-repeat: repeat-x;
      background-size: contain;
      position: absolute;
      top: 660px;
    }
    .home-Title_Elephants {
      z-index: 3;
      position: absolute;
      top: 680px;
      right: calc(50vw - 205px);
      background: right;
      text-align: right;
    }
    .home-Title_Elephant {
      display: inline-block;
      width: 112px;
      height: 98px;
      background-image: url("/images/elephant.png");
      background-repeat: no-repeat;
      background-size: contain;
    }
    .home-Title_Attention {
      padding: 1rem;
      border-radius: 1rem;
      font-size: 18px;
      font-weight: bold;
      color: $clr_base;
      text-decoration: none;
      text-align: center;
      background: $clr_accent;
      position: relative;
      top: -130px;
      &::after {
         display: inline-block;
         content: "";
         width: 20px;
         height: 20px;
         background-image: url("/images/parts_triangle.svg");
         background-repeat: no-repeat;
         background-size: contain;
         position: absolute;
         top:42px;
         right: 20px;
       }
    }
  }
</style>
