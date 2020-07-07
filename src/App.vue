<template>
  <div id="app">
    <v-header :seller="seller"></v-header>
    <header-detail :seller="seller"></header-detail>
  </div>
</template>

<script>
  import VHeader from './components/v-header/v-header'
  import HeaderDetail from './components/header-detail/header-detail'
  import {getSeller} from 'api'

  export default {
    name: 'App',
    data() {
      return {
        seller: {}
      }
    },
    created() {
      this._getSeller()
    },
    methods: {
      _getSeller() {
        getSeller().then((seller) => {
          // 由于用 axios 封装了一遍，这里一定可以拿到数据
          this.seller = seller
        })
      }
    },
    components: {
      HeaderDetail,
      VHeader
    }
  }
</script>

<style lang="stylus">
</style>
