<template>
    <div class="outer">
        <div class="inner">
            <h1 class="title"> {{ title }}</h1>
        </div>
        <div class="border"></div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            title: "宁·空间"
        }
    }
}
</script>
<style scoped>
.outer {
    width: 100%;
    height: 100%;
}
.inner {
    width: 100%;
    height: 95%;
}
.title {
    margin: 0;
    font-size: 28px;
    font-weight: lighter;
    color: rgb(250, 179, 151);
    letter-spacing: 10px;
}
.border {
    width: 100%;
    height: 5%;
    background: linear-gradient(
        to right,
        #fff,
        rgb(254, 191, 191),
        #fff 
    );
}
</style>