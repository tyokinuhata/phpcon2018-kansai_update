<template>
  <div class="home-Access">
    <div class="home-Access_Wave"></div>
    <div class="st-Container">
      <h2 class="home-Access_Title">ACCESS</h2>
      <no-ssr>
        <googlemaps-map ref="map" :center="center" @ready="ready" class="home-Access_Map"></googlemaps-map>
      </no-ssr>
      <div class="home-Access_Map" id="map"></div> <!-- ここにGoogle Mapsが入ります -->
      <div class="home-Access_Description">
        <p class="home-Access_Place">グランフロント大阪&nbsp;北館&nbsp;タワーC&nbsp;8階</p>
        <p class="home-Access_Address">〒530-0011&nbsp;大阪市北区大深町3-1<br>&nbsp;グランフロント大阪&nbsp;北館&nbsp;タワーC8階</p>
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

<script>
  export default {
    data () {
      return {
        center: { lat: 0, lng: 0 }
      }
    },
    methods: {
      ready () {
        this.$refs.map.resize()
      }
    }
  }
</script>

<style lang="scss" scoped>
  @import "~assets/scss/library/_variable.scss";
  @import "~assets/scss/library/_mixin.scss";

  .home-Access {
    padding: 70px 0 70px 0;
    width: auto;
    background-color: $clr_main;

    &_Wave {
      width: 100%;
      height: 20px;
      background-image: url("/images/wavyLine-keyColor.png");
      background-repeat: repeat-x;
      background-size: contain;
      position: relative;
      top: -90px;
    }

    &_Title {
      @include secTitle;
      margin-bottom: 30px;
    }

    &_Map {
      max-width: 900px;
      width: 100%;
      height: 250px;
      margin: 0 auto;
      margin-bottom: 15px;
      /*background: #ccc;*/

      @include desktop() {
        margin-bottom: 30px;
        height: 400px;
      }
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
      margin: 0 5px 10px 5px;
      width: 200px;
      @include desktop() {
        margin: 0 0 10px 5px;
      }
    }
  }
</style>
