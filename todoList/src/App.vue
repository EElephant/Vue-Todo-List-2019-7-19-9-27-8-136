<template>
  <div id="app">
    <Header></Header>
    <Body></Body>
    <Footer></Footer>
  </div>
</template>

<script>
import Header from './components/Header'
import Body from './components/Body'
import Footer from './components/Footer'

export default {
  name: 'App',
  components:{
    Header,
    Body,
    Footer
  }
}
</script>

<style>
#app {
  padding: 20px;
  width: 600px;
  margin: 0 auto;
  margin-top: 40px;
  background: white;
  border-radius: 5px;
}
</style>
