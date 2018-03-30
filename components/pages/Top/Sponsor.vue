<template>
  <div class="home-Sponsor">
    <div class="st-Container">
      <h2 class="home-Sponsor_Title">SPONSOR</h2>
      <p class="home-Sponsor_Description">初心者から上級者まで楽しめるセッションが目白押し！これから始めようと思っていたフレームワークや、気になっていた技術についての情報が得られるかも！？</p>
      <div class="home-Sponsor_Sponsor">
        <div class="home-Sponsor_Platinum">
          <h3>プラチナスポンサー</h3>
          <div class="home-Sponsor_Large"></div>
          <div class="home-Sponsor_Large"></div>
        </div>
        <div class="home-Sponsor_Gold">
          <h3>ゴールドスポンサー</h3>
          <div class="home-Sponsor_Medium"></div>
          <div class="home-Sponsor_Medium"></div>
          <div class="home-Sponsor_Medium"></div>
          <div class="home-Sponsor_Medium"></div>
          <div class="home-Sponsor_Medium"></div>
          <div class="home-Sponsor_Medium"></div>
          <div class="home-Sponsor_Medium"></div>
          <div class="home-Sponsor_Medium"></div>
        </div>
        <div class="home-Sponsor_Silver">
          <h3>シルバースポンサー</h3>
          <div class="home-Sponsor_Small"></div>
          <div class="home-Sponsor_Small"></div>
          <div class="home-Sponsor_Small"></div>
          <div class="home-Sponsor_Small"></div>
          <div class="home-Sponsor_Small"></div>
          <div class="home-Sponsor_Small"></div>
          <div class="home-Sponsor_Small"></div>
          <div class="home-Sponsor_Small"></div>
          <div class="home-Sponsor_Small"></div>
          <div class="home-Sponsor_Small"></div>
        </div>
        <div class="home-Sponsor_Media">
          <h3>メディアスポンサー</h3>
          <div class="home-Sponsor_Small"></div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  @import "~assets/scss/library/_variable.scss";
  @import "~assets/scss/library/_mixin.scss";

  .home-Sponsor {
    padding: 70px 0 70px 0;
    width: auto;
    background: $clr_baseDark;

    &_Title {
      @include secTitle;
    }

    &_Description {
      max-width: 770px;
      width: 100%;
      margin: 0 auto;
      padding: 0 0 30px 0;
    }

    &_Large {
      display: inline-block;
      max-width: 440px;
      width: 100%;
      height: 260px;
      background: $clr_baseWhite;

      @include desktop() {
        &:nth-child(2) {
          margin-right: 15px;
        }

        &:nth-child(3) {
          margin-left: 15px;
        }
      }
    }

    &_Medium {
      display: inline-block;
      max-width: 210px;
      width: 100%;
      height: 140px;
      background: $clr_baseWhite;

      @include desktop() {

        &:not(first-child) {
          margin: 0 10px;
        }
      }
    }

    &_Small {
      display: inline-block;
      max-width: 150px;
      width: 100%;
      height: 100px;
      background: $clr_baseWhite;

      @include desktop() {

        &:not(first-child) {
          margin: 0 10px;
        }
      }
    }
  }
</style>
