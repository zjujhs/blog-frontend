<template>
    <div class="outer">
        <div style="flex:1"></div>
        <div class="carousel-block">
            <el-carousel :interval="4000" class="carousel" height="500px">
                <el-carousel-item 
                    v-for="(value, index) in a" 
                    :key="index"
                    :style="{'background-image': 'url('+value+')'}"
                    class="carousel-item"
                >
                    <div class="carousel-title-block">
                        <p class="carousel-title">奥斯卡的哈看手机德哈卡山东科技安徽省打卡机阿萨德</p>
                    </div>
                </el-carousel-item>
            </el-carousel>
        </div>
        <div class="titles">
            <div class="titles-inner">
                <div class="title-block" v-for="(value, index) in b" :key="index">
                    <div class="pot-div">
                        <div class="pot"></div>
                    </div>
                    <p class="title">{{ value }}</p>
                    <p class="date">xxxx-xx-xx</p>
                </div>
            </div>
        </div>
        <div style="flex:1"></div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            a: [
                '/tmp.png',
                '/guohui.png'
            ],
            b: [
                '爱德华发生了客服号的沙拉护发看傻了都发哈萨克斯',
                '阿达独立董事会计法哈拉少快递费活动实例咖啡机',
                '看哈流动商贩就好看撒旦法回拉萨款到发货山卡拉多加防护烧腊店发哈开始的',
                '安居客都会发送浪费哈萨克的房间哈三联开发了可接收的父类建安费',
                '会计核算打开了发哈释放空间的身份雷克萨兑换积分临时卡接化发冷风机'
            ]
        }
    },
    mounted() {

    }
}
</script>
<style scoped>
.outer {
    width: 100%;
    display: flex;
}
.carousel-block {
    flex: 11;
}
.titles {
    flex: 11;
    /* background-color: #888; */
    display: flex;
    justify-content: center;
    align-items: center;
    border-left: 1px solid transparent;
    border-image: linear-gradient(
        to bottom,
        white,
        rgb(31, 90, 153),
        rgb(92, 153, 219),
        white
    ) 30;
}
.titles-inner {
    width: 80%;
    height: 80%;
    display: flex;
    flex-direction: column;
}
.title-block {
    flex: 1;
    display: flex;
    align-items: center;
}
.title {
    flex: 18;
    margin: 0;
    text-align: left;
    font-size: large;
    letter-spacing: 2px;
    font-weight: lighter;
}
.pot-div {
    flex: 1;
    height: 100%;
    display: flex;
    justify-content: left;
    align-items: center;
}
.pot {
    height: 10px;
    width: 10px;
    border-radius: 5px;
    background: linear-gradient(
        to bottom,
        rgb(31, 90, 153),
        rgb(92, 153, 219)
    );
}
.date {
    flex: 5;
    margin: 0;
    text-align: right;
}
@import url('/src/style/carousel.css');
</style>