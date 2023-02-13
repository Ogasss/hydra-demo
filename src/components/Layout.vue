<template>
<div class="theLayoutWrapper">
    <div class="theTopNav">
        <TopNav/>
    </div>
    <div class="theMain">
        <Dive/>
    </div>
</div>
</template>

<script>
import TopNav from './TopNav/TopNav.vue'
import Dive from './Main/Dive.vue'
export default {
    components:{
        TopNav,
        Dive
    },
}
</script>

<style scoped>
.theLayoutWrapper{
    width: 100%;
    min-width: 1324px;
    height: 5597px;
}
.theTopNav{
    position: fixed;
    top: 0px;
    width: 100%;
    z-index: 2;
}
.theMain{
    position: relative;
    z-index: 1;
}
</style>