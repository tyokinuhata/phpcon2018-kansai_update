<template>
  <div class="home-Sponsor">
    <div class="st-Container">
      <h2 class="home-Sponsor_Title">SPONSOR</h2>
      <p class="home-Sponsor_Description">初心者から上級者まで楽しめるセッションが目白押し！これから始めようと思っていたフレームワークや、気になっていた技術についての情報が得られるかも！？</p>
      <div class="home-Sponsor_Sponsor">
        <div class="home-Sponsor_Platinum">
          <h3>プラチナスポンサー</h3>
          <div></div>
          <div></div>
        </div>
        <div class="home-Sponsor_Gold">
          <h3>ゴールドスポンサー</h3>
          <div></div>
          <div></div>
          <div></div>
          <div></div>
          <div></div>
          <div></div>
          <div></div>
          <div></div>
        </div>
        <div class="home-Sponsor_Silver">
          <h3>シルバースポンサー</h3>
          <div></div>
          <div></div>
          <div></div>
          <div></div>
          <div></div>
          <div></div>
          <div></div>
          <div></div>
          <div></div>
          <div></div>
        </div>
        <div class="home-Sponsor_Media">
          <h3>メディアスポンサー</h3>
          <div></div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  @import "~assets/scss/library/_variable.scss";
  @import "~assets/scss/library/_mixin.scss";

  .home-Sponsor {
    padding: 130px 0 70px 0;
    width: auto;
    background: $clr_baseDark;

    &_Title {
      @include secTitle;
    }
  }
</style>
