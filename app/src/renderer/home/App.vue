<template>
  <div id="#app">
    <main-header/>
    <main-board>
      <left-panel slot="left"/>
      <router-view slot="right"></router-view>
    </main-board>
    <main-footer/>
    <player/>
  </div>
</template>

<script>
  import store from '@renderer/home/vuex/store'
  import MainHeader from '@components/MainHeader'
  import MainFooter from '@components/MainFooter'
  import MainBoard from '@components/MainBoard'
  import LeftPanel from '@components/LeftPanel'
  import Player from '@components/Player'
  export default {
    store,
    components: {
      MainHeader,
      MainFooter,
      MainBoard,
      LeftPanel,
      Player
    },
    created() {
    }
  }
</script>

<style>
@import '../@common/basic';
@import '../@common/icon';
</style>
