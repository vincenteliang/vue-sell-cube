<template>
  <div id="app">
    <v-header :seller="seller"></v-header>
    <div class="tab-wrapper">
      <tab :tabs="tabs"></tab>
    </div>
  </div>
</template>

<script>
  import VHeader from 'components/v-header/v-header'
  import {getSeller} from 'api'
  // import Goods from 'components/goods/goods'
  // import Ratings from 'components/ratings/ratings'
  // import Seller from 'components/seller/seller'
  import Tab from 'components/tab/tab'

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
      VHeader,
      Tab
    }
  }
</script>

<style lang="stylus">
</style>
