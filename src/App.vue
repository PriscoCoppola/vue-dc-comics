<template>
  <div id="app">
    <div class="container">
      <Header/>

      <main>
        <Content/>

        <Products/>
      </main> 

      <Footer/>   
    </div>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Content from './components/Content.vue'
import Products from './components/Products.vue'
import Footer from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    Header,
    Content,
    Products,
    Footer,
  }
}
</script>

<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: sans-serif;
  }
</style>
