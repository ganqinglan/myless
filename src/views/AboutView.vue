<template>
  <div class="about">
       <div class="wraper">
           <div class="inner">
              <div class="ragtangle"></div>
           </div>
       </div>

       <Demo></Demo>
  </div>
</template>
<script>
import Demo from '@/components/demo.vue'
export default {
  components:{
    Demo
  }
}
</script>
<style lang="less" scoped>
.all{
   width:0px;
      height: 0px;
      overflow: hidden;
}
.wraper{
  width:400px;
  height: 400px;
  background-color: aqua;
  color: white;
  margin:0 auto;

  .inner{
    width: 200px;
    height: 200px;
    border: 2px solid blueviolet;
    .ragtangle{
       .all;
      .triangle(bottom);
    }
  }
}

// 匹配模式
@w:width;
@c:color;
// 上三角
.triangle(top,@w:10px,@c:red){
      border-width: @w;
      border-color: transparent transparent red transparent;
      border-style: dashed dashed solid dashed;
}
// 右三角
.triangle(right,@w:10px,@c:red){
   border-width: @w;
      border-color: transparent transparent  transparent red;
      border-style: dashed dashed  dashed solid;
}
// 下三角
.triangle(bottom,@w:10px,@c:red){
   border-width: @w;
      border-color: red transparent transparent  transparent ;
      border-style:  solid dashed dashed  dashed;
}


</style>
