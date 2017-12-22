<template>
  <div>
    <m-header :isReturn="false"></m-header>
    <div>
      <nuxt-link to="/home/pay">自助交费</nuxt-link>
      <nuxt-link to="/home/appoint">预约车位</nuxt-link>
    </div>
  </div> 
</template>

<script>
import mHeader from '~/components/mHeader.vue'
export default {
  components: {
    mHeader
  }
}
</script>

<style>
</style>
