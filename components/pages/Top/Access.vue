<template>
  <div class="home-Access">
    <div class="st-Container">
      <h2 class="home-Access_Title">ACCESS</h2>
      <div class="home-Access_Map"></div>
      <div class="gome-Access_Description">
        <p>グランフロント大阪&nbsp;北館&nbsp;タワーC&nbsp;8階</p>
        <p>〒530-0011&nbsp;大阪市北区大深町3-1<br>&nbsp;グランフロント大阪&nbsp;タワーC8階</p>
        <p>
          <i class="far fa-calendar-check"></i>
          <span>タワーCへはグランフロント北館1階からしかアクセスできません</span>
        </p>
      </div>
      <div class="home-Access_Link">
        <a href="https://twitter.com/phpcon_kansai" target="_blank" class="home-Access_Google">
          <i class="far fa-calendar-check"></i>
          <span>&nbsp;Googleマップを開く</span>
        </a>
        <a href="https://twitter.com/phpcon_kansai" target="_blank" class="home-Access_Detail">
          <i class="far fa-calendar-check"></i>
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
    padding: 130px 0 70px 0;
    width: auto;
    background-color: #58C0AE;

    &_Title {
      @include secTitle;
    }

    &_Google, &_Detail {
      @include button;
    }
  }
</style>
