<template>
  <div class="home-Share">
    <div class="st-Container">
      <h2 class="home-Share_Title">Share on SNS</h2>
      <p class="home-Share_Description">ワクワクをシェアしよう！<br>イベントに関する要望等もお待ちしております。</p>
      <div class="home-Share_List">
        <div class="home-Share_Twitter"><a href="https://twitter.com/intent/tweet?text=関西最大のPHPイベントは7月14日(土)にグランフロント大阪にて開催! PHPカンファレンス関西2018 https://2018.kphpug.jp&amp;hashtags=phpkansai" target="_blank">twitterでつぶやく</a><i class="fa fa-twitter fa-2x" aria-hidden="true"></i></div>
        <div class="home-Share_Facebook"><a href="https://www.facebook.com/sharer.php?u=https://2018.kphpug.jp&amp;amp;t=関西最大のPHPイベントは7月14日(土)にグランフロント大阪にて開催! PHPカンファレンス関西2018&amp;hashtags=phpkansai" target="_blank">Facebookでシェア</a><i class="fa fa-facebook fa-2x" aria-hidden="true"></i></div>
      </div>
    </div>
  </div>
</template>

<script>

</script>

<style lang="scss" scoped>
  @import "~assets/scss/library/_variable.scss";
  @import "~assets/scss/library/_mixin.scss";

  .home-Share {
    padding: 70px 0;
    width: auto;
    background-color: #00C5AC;

    &_Title {
      @include secTitle();
    }
    &_Description {

    }
    .home-Share_List {
      margin-top: 30px;
      color: $clr_base;

      .home-Share_Twitter {
        @include buttonSns;
      }

      .home-Share_Facebook {
        @include buttonSns;
      }
    }
  }

</style>
