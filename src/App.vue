<template>
  <div id="app">
    <v-header :seller="seller"></v-header>
  </div>
</template>

<script>
  import VHeader from './components/v-header/v-header'
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
      VHeader
    }
  }
</script>

<style lang="stylus">
</style>
