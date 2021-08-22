<template>
  <div>
    <h2>Current prices</h2>
    <div id="btc" class="currency">
      <label>1 BTC</label>
      <p>${{currentCurrency.BTC}}</p>
    </div>
    <div id="eth"class="currency">
      <label>1 ETH</label>
      <p>${{currentCurrency.ETH}}</p>
    </div>
    <div id="usd"class="currency">
      <label>1 USD</label>
      <p>${{currentCurrency.USD}}</p>
    </div>
    <div id="eur"class="currency">
      <label>1 EURO</label>
      <p>${{currentCurrency.EUR}}</p>
    </div>
  </div>
</template>

<script>
  export default {
    name: 'app',
    props: {
      currentCurrency: {
        type: Object
      }
    },
    data() {
      return {

      }
    }
  }
</script>

<style scoped>
  .currency {
    border: 1px solid #F5CE00;
    border-radius: 15px;
    padding: 2em 0em;
    display: inline-block;
    width: 30%;
  }
  div p { font-size: 2rem; }
  h2 { font-size: 1.5em; }
</style>
