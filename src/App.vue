<template>
  <div id="app">
    <el-container>
      <el-header><page-header></page-header></el-header>
    </el-container>
    <div><router-view></router-view></div>
  </div>
</template>

<script>
import pageHeader from './components/pageHeader.vue'
import pageSearch from './components/pageSearch.vue'
import pageCard from './components/pageCard.vue'
import pageStar from './components/pageStar.vue'
import pageShowStar from './components/pageShowStar.vue'
import pagePlayCard from './components/pagePlayCard.vue'
export default {
  name: 'App',
  components: {
    'page-header': pageHeader,
    'page-search': pageSearch,
    'page-card': pageCard,
    'page-star': pageStar,
    'page-showstar': pageShowStar,
    'page-playcard': pagePlayCard
  }
}
</script>

<style>
#search-bar{
  position: absolute;
  top: 0;
}
.el-footer{
  position: absolute;
  bottom: 0;
}
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
  padding-top: 0;

}
</style>
