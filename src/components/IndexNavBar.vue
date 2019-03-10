<template>
  <a href="#tab1" class="tab-link button active" style="background-color: rgb(255, 45, 45);">
    <div class="gift-icon">
      <div class="icon1"><img src="http://smsptest.mypicc.com.cn/WebTransNet4/$bjadmin/bjwxplat/dzsw/dszh/images/1-white.png"></div>
      <div class="theme1"><span style="color: rgb(255, 255, 255);">我的福袋</span></div>
    </div>
  </a>
</template>

<script>
export default {
  name: 'IndexNavBar'  
}
</script>

<style scoped>
.icon1{
  height: 2rem;
  display: flex;
  justify-content: center;
  align-items: center;
}
.theme1{
  height: .4rem;
  display: flex;
  align-items: center;
  justify-content: center;
}
.img{
  border: 0;
  width: .6rem;
  height: .6rem;
}
</style>
