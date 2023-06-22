<template>
    <div class="outer">
        <div class="header">
            <pageHeader/>
        </div>
        <div class="main">

        </div>
    </div>
</template>
<script>
import pageHeader from "@/components/PageHeader.vue"
export default {
    components: {
        pageHeader,
    }
}
</script>
<style scoped>
.outer, .header, .main {
    width: 100%;
}
.outer {
    height: 100vh;
    /* background-color: #111; */
}
.header {
    height: 50%;
    background-color: #222;
}
.main {
    height: 50%;
    /* background-color: #333; */
}
</style>