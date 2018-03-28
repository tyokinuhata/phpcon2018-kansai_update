<template>
  <section class="container">
    <sec-hero></sec-hero>
    <sec-about></sec-about>
    <sec-time-table></sec-time-table>
    <sec-access></sec-access>
    <sec-sponsor></sec-sponsor>
    <sec-share></sec-share>
    <sec-follow></sec-follow>
    <p-footer></p-footer>
  </section>
</template>

<script>
  import secHero from '~/components/pages/Top/Hero.vue'
  import secAbout from '~/components/pages/Top/About.vue'
  import secTimeTable from '~/components/pages/Top/TimeTable.vue'
  import secAccess from '~/components/pages/Top/Access.vue'
  import secSponsor from '~/components/pages/Top/Sponsor.vue'
  import secShare from '~/components/pages/Top/Share.vue'
  import secFollow from '~/components/pages/Top/Follow.vue'
  import pFooter from '~/components/Footer.vue'

  export default{
      components:{
          secHero,
          secAbout,
          secTimeTable,
          secAccess,
          secSponsor,
          secShare,
          secFollow,
          pFooter
      }
  }

</script>

<style>
@import "normalize.css";
</style>
