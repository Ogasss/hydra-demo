<template>
<div class="theLayoutWrapper">
    <div class="theTopNav">
        <TopNav/>
    </div>
    <div class="theMain">
        <Dive/>
        <Introduction/>
    </div>
</div>
</template>

<script>
import TopNav from './TopNav/TopNav.vue'
import Dive from './Main/Dive.vue'
import Introduction from './Main/Introduction.vue'
export default {
    components:{
        TopNav,
        Dive,
        Introduction
    },
}
</script>

<style scoped>
.theLayoutWrapper{
    width: 100%;
    min-width: 1485px;
    height: 5597px;
}
.theTopNav{
    position: fixed;
    top: 0px;
    width: 100%;
    z-index: 2;
}
.theMain{
    padding: 0px 84px;
    position: relative;
    z-index: 1;
}
</style>