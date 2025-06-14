<template>
  <div id="app" >
    <MainHeader/>
    <MainBlock/>
  </div>
</template>

<script>
import MainHeader from './components/MainHeader.vue'
import MainBlock from './components/MainBlock.vue'

export default {
  name: 'App',
  components: {
    MainHeader,
    MainBlock,
  }
}
</script>
