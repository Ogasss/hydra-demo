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
    height: 5597px;
}
.theTopNav{
    position: fixed;
    top: 0px;
    width: 100%;
}
.theMain{
}
</style>