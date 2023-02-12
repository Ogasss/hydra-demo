<template>
<div class="theLayoutWrapper">
    <div class="theTopNav">
        <TopNav/>
    </div>
    <div class="theMain">

    </div>
</div>
</template>

<script>
import TopNav from './TopNav/TopNav.vue'
export default {
    components:{
        TopNav,
    },
    setup(){
    }
}
</script>

<style scoped>
.theLayoutWrapper{
    width: 100%;
}
.theTopNav{
    position: fixed;
    top: 0px;
    width: 100%;
}
.theMain{
}
</style>