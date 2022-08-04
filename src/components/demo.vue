<template>
    <div id="">
        <p>demo</p>
        <ul>
            <li><a>支付</a></li>
            <li><a>微信</a></li>
            <li><a>支付宝</a></li>
            <li><a>数字人民币</a></li>
        </ul>
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

<style scoped lang="less">
  ul{
    width: 200px;
    height: 200px;
    background-color: antiquewhite;
    li{
        list-style-type: circle;
        a{
            color:red;
            // &  :表示的是上一级的选择器
            &:hover{
                color: blueviolet;
            }
        }
    }
  }
</style>
