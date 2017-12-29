<template>
  <div>
    <m-header><span>预约车位</span></m-header>
    <div class="container">
      <search></search>
    </div>
  </div>
</template>
<script>
import mHeader from '~/components/mHeader.vue'
import search from '~/components/search.vue'

export default {
  components: {
    mHeader,
    search
  }
}
</script>