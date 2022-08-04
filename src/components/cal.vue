<template>
    <div id="">
           <div class="container">
              <div class="inner"></div>
           </div>
    </div>
</template>

<script >
export default {
    name: "",
    data() {
        return {}
    },
    components: {},
    methods: {}
}
</script>

<style lang="less" scoped>
@w:300px;
@h:500px;
.container{
   width:@w+100;
   height:@h - 100 ;
   .inner{
    width: @w/2;
    height: @h/2;
   }
}
</style>
