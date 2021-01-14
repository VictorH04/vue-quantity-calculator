<template>
  <div id="app">

    <Header />

    <QuantityInput />

    <QuantityResult v-bind:inputs="quantityResult" />
    
     <!-- v-bind:inputs="quantityResult" -->
  </div>
</template>

<script>
import Header from './components/layout/Header.vue';
import QuantityResult from './components/QuantityResult.vue';
import QuantityInput from './components/QuantityInput.vue';


export default {

  name: 'App',
  components: {
    Header,
    QuantityResult,
    QuantityInput
  },

  data() {

    return {
      quantityResult: [

        {
          id: 1,
          quanInput: 'Lengde'
        },

        {
          id: 2,
          quanInput: 'Bredde'
        },

        {
          id: 3,
          quanInput: 'Tykkelse'
        },

        {
          id: 4,
          quanResult: '0 cm^3'
        }

      ]

    }
  }

}
</script>

<style>

* {
  box-sizing: inherit;
  margin: 0;
  padding: 0;
}

html {
  font-size: 62.5%;
  box-sizing: border-box;
}

body {
  box-sizing: border-box;
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.4;
}


</style>
