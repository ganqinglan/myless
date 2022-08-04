<template>
  <div class="hello">
      <div class="container">
           <div class="inner">
              <ul>
                <li>江西</li>
                <li>宜春</li>
                <li>万载</li>
                <li>朱熹</li>
              </ul>
           </div>
      </div>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="less">
@w:400px;
@c:color;
@value:rgb(195, 104, 14);
.class{
  border: 2px solid blue;
}
.bg(@bgc:red){
  background-color:@bgc;
}
.container{
  width: @w;
  height: 400px;
  @{c}:@value;
  // .bg(green);
  .bg();
  margin:0 auto;
  .class;
     .inner{
         border: 1px solid red;
     }
}




</style>
