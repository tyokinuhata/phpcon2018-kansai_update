<template>
  <div class="home-Follow">
    <div class="st-Container">
      <h2 class="home-Follow_Title">Follow SNS</h2>
      <p>PHPカンファレンス関西のSNSアカウントをフォローして<br/>最新情報チェック！</p>
      <div class="home-Follow_SNS">
        <a href="https://twitter.com/phpcon_kansai" target="_blank" class="home-Follow_Twitter">
          <i aria-hidden="true" class="fa fa-twitter fa-lg"></i>
          <span>&nbsp;twitterアカウント</span>
        </a>
        <a href="https://www.facebook.com/pcon.kansai/" target="_blank" class="home-Follow_Facebook">
          <i aria-hidden="true" class="fa fa-facebook fa-lg"></i>
          <span>&nbsp;Facebookグループ</span>
        </a>
      </div>
    </div>
  </div>
</template>

<script>
</script>

<style lang="scss" scoped>
  @import "~assets/scss/library/_variable.scss";
  @import "~assets/scss/library/_mixin.scss";

  .home-Follow {
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
