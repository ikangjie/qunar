<template>
  <div>
    <div class="content">
      <detail-banner></detail-banner>
    </div>
  </div>
</template>

<script>
import DetailBanner from './commponents/Banner'
export default {
  name: 'Detail',
  components: {
    DetailBanner
  }
}
</script>

<style lang="stylus" scoped>
  .content
    height: 50rem
</style>
