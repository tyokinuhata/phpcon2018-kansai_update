<template>
  <div class="home-Access">
    <div class="st-Container">
      <h2 class="home-Access_Title">ACCESS</h2>
      <div class="home-Access_Map">ここにGoogle Mapsが入ります</div>
      <div class="home-Access_Description">
        <p class="home-Access_Place">グランフロント大阪&nbsp;北館&nbsp;タワーC&nbsp;8階</p>
        <p class="home-Access_Address">〒530-0011&nbsp;大阪市北区大深町3-1<br>&nbsp;グランフロント大阪&nbsp;タワーC8階</p>
        <p class="home-Access_Warn">
          <i class="fa fa-exclamation-triangle" aria-hidden="true"></i>
          <span>&nbsp;タワーCへはグランフロント北館1階からしかアクセスできません</span>
        </p>
      </div>
      <div class="home-Access_Link">
        <a href="https://twitter.com/phpcon_kansai" target="_blank" class="home-Access_Google">
          <i class="fa fa-map-marker" aria-hidden="true"></i>
          <span>&nbsp;Googleマップを開く</span>
        </a>
        <a href="https://twitter.com/phpcon_kansai" target="_blank" class="home-Access_Detail">
          <i class="fa fa-map" aria-hidden="true"></i>
          <span>&nbsp;タワーC&nbsp;アクセス詳細</span>
        </a>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped>
  @import "~assets/scss/library/_variable.scss";
  @import "~assets/scss/library/_mixin.scss";

  .home-Access {
    padding: 70px 0 70px 0;
    width: auto;
    background-color: $clr_main;

    &_Title {
      @include secTitle;
      margin-bottom: 30px;
    }

    &_Map {
      max-width: 900px;
      width: 100%;
      height: 400px;
      margin: 0 auto;
      margin-bottom: 30px;
      background: #ccc;
    }

    &_Description {
      margin-bottom: 30px;
    }

    &_Place {
      margin-bottom: 20px;
    }

    &_Address {
      margin-bottom: 30px;
    }

    &_Warn {

    }

    &_Google, &_Detail {
      @include button;
    }
  }
</style>
