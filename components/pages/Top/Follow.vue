<template>
  <div class="p-follow">
    <div class="c-ontainer">
      <h2 class="home-Follow_Title">Follow SNS</h2>
      <p>PHPカンファレンス関西のSNSアカウントをフォローして<br>最新情報チェック！</p>
      <div class="home-Follow_SNS"><a class="home-Follow_Twitter" href="https://twitter.com/phpcon_kansai" target="_blank"><i class="fa fa-twitter fa-lg" aria-hidden="true"></i><span>&nbsp;twitterアカウント</span></a><a class="home-Follow_Facebook" href="https://www.facebook.com/pcon.kansai/" target="_blank"><i class="fa fa-facebook fa-lg" aria-hidden="true"></i><span>&nbsp;Facebookグループ</span></a></div>
    </div>
  </div>
</template>

<script>
</script>

<style lang="scss" scoped>
  @import "~assets/scss/library/_variable.scss";
  @import "~assets/scss/library/_mixin.scss";
  .p-follow {
    width: auto;
    color: $clr_base;
    background-color: #fff;
    padding: 70px 0;

    &_Title {
      @include secTitle($clr_base);
     }

    &_SNS {
       margin-top: 40px;
      .home-Follow_Twitter {
        @include button();
      }
    .home-Follow_Facebook {
        @include button();
      }
    }
  }
</style>
