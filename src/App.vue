<template>
  <svg class="logo" xmlns="http://www.w3.org/2000/svg" width="23.991" height="23.433" viewBox="0 0 23.991 23.433"><defs></defs><path fill="#01d167" d="M23.5,14.772c0,.067,0,.133-.069.133a.149.149,0,0,1-.138-.133c-.207-.266-10.675-11.323-11.157-11.723-.207-.2-.275-.133-.482.067C11.588,3.182.707,14.639.569,14.838c-.069.067-.138.067-.138-.067a10.912,10.912,0,0,1-.413-3.663A10.341,10.341,0,0,1,1.533,6.046,11.451,11.451,0,0,1,9.384.318,11.829,11.829,0,0,1,20.61,3.582a10.907,10.907,0,0,1,3.237,6.261,8.818,8.818,0,0,1,.138,1.932A15.1,15.1,0,0,1,23.5,14.772Z" transform="translate(0 0)"/><path fill="#01d167" d="M.08,9.109c-.069-.067-.138-.133,0-.266S8.275.25,8.482.05c.069-.067.138-.067.138,0,.275.333,8.2,8.726,8.4,8.859.069.067.069.133-.069.133a9.34,9.34,0,0,1-1.515,1.266,11.776,11.776,0,0,1-5.923,2.131,6.121,6.121,0,0,1-1.1.067A11.907,11.907,0,0,1,.08,9.109Z" transform="translate(3.451 10.925)"/></svg>
  <cards/>
  <debit-card/>
  <div class="drawer">
    <quick-links/>
    <card-details/>
    <recent-transactions/>
  </div> 
  <bottom-nav/>
</template>

<script>
import Cards from './components/Cards.vue'
import BottomNav from './components/BottomNav.vue'
import CardDetails from './components/CardDetails.vue'
import QuickLinks from './components/QuickLinks.vue'
import RecentTransactions from './components/RecentTransactions.vue'
import DebitCard from './components/DebitCard.vue'

export default {
  name: 'App',
  components: {
    Cards,
    BottomNav,
    CardDetails,
    RecentTransactions,
    QuickLinks,
    DebitCard
  }
}
</script>

<style lang="scss">
@import "@/assets/styles/variables.scss";
@import './assets/styles/style.scss';
.logo{
  position: fixed;
  z-index: 1;
  right:24px;
  top: 24px;
  @media (min-width: $md) {
    display: none;
  }
}
.drawer{
  background: $color-white;
  border-top-left-radius: 15px;
  border-top-right-radius: 15px;
  position: absolute;
  z-index: 1;
  width: 100%;
  left: 0;
  top: 55vh;
  padding-bottom: 70px;
  @media (min-width: $md) {
    position: static;
    margin-left: 400px;
    width:calc(100% - 400px);
    padding: 24px;
  }
}
</style>