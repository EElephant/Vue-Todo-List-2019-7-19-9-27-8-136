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

let id=0;
const getId = () => {
  return id++;
}

export default {
  name: 'App',
  methods:{
      returnList(val){
        const item= {
          val,
          id:getId(),
          editable: false
        }
        this.list.push(item)
      }
  },
  components:{
    Header,
    Body,
    Footer
  },
  computed: {
    list () {
      return this.$store.state.allItems;
    }
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
