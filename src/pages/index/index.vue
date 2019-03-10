<template>
<div id="app">
  <mt-navbar v-model="selected">
    <mt-tab-item id="1">
      <index-nav-bar></index-nav-bar>
    </mt-tab-item>
    <mt-tab-item id="2">选项二</mt-tab-item>
    <mt-tab-item id="3">选项三</mt-tab-item>
    <mt-tab-item id="4">选项四</mt-tab-item>
  </mt-navbar>

  <!-- tab-container -->
  <mt-tab-container v-model="selected">
    <mt-tab-container-item id="1">
      <mt-cell v-for="n in 10" :title="'内容 ' + n" />
    </mt-tab-container-item>
    <mt-tab-container-item id="2">
      <mt-cell v-for="n in 4" :title="'测试 ' + n" />
    </mt-tab-container-item>
    <mt-tab-container-item id="3">
      <mt-cell v-for="n in 6" :title="'选项 ' + n" />
    </mt-tab-container-item>
  </mt-tab-container>
</div>
</template>

<script>
import IndexNavBar from '@/components/IndexNavBar'


export default {
  name: 'index'
  ,components:{
    IndexNavBar
  }
  ,data(){
    return {
      selected:'1'  
    }
  },
  mounted(){

  }
  // ,props: ['message']
  ,methods:{
    handleClose(){
      alert('handleClose')
    }
  }
}
</script>

<style scoped>
#app{
  max-width: 640px;
  margin: 0 auto;
}
.mint-tab-item{
    height: 1.38rem;
    font-size: .8rem;
    line-height: 3.5rem;
    color: #5f646e;
    border: 0;
    border-bottom: 2px solid transparent;
    border-radius: 0;
    -webkit-box-flex: 1;
    -ms-flex: 1;
    padding: 0
}
.mint-tab-item.is-selected{
  color: #ad0f00;
  border-color: #ad0f00;
  background-color:rgb(255, 45, 45);
}
</style>
