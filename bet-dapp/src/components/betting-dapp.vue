<template>
<div>
  <DappMetamask />
  <BettingComponent />
</div>
</template>
<script>
import DappMetamask from '@/components/dapp-metamask'
import BettingComponent from '@/components/betting-component'
export default {
  name: 'betting-dapp',
  beforeCreate() {
    /*eslint-disable no-console*/
    console.log('registerWeb3 Action dispatched')
    this.$store.dispatch('registerWeb3')
  },
  components: {
    DappMetamask,
    BettingComponent
  }
}
</script>
<style scoped>
</style>
