<template>
    <div class="theBallItem">
        <div class="ballWrapper">
            <Button class="ball" ball>
                <slot name="number"></slot>
            </Button>
        </div>
        
        <div class="textPart">
            <img class="right" :src="right" alt="">
            <div class="text">
                <slot name="text"></slot>
            </div>
        </div>
    </div>
</template>

<script>
import right from '../../assets/right.svg'
import Button from '../shared/button.vue'
export default {
    components:{
        Button
    },
    setup(){
        return{
            right
        }
    }
}
</script>

<style scoped>
    .theBallItem{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
    .ballWrapper{
        width: 198px;
        height: 198px;
        background: #0D0D0D52;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 50%;
        margin-bottom: 25px;
    }
    .ball{
        width: 159px;
        height: 159px;
    }
    .textPart{
        display: flex;
    }
    .textPart .text{
        margin-left: 15.54px;
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 700;
        font-size: 24px;
        line-height: 29px;
        color: #FFFFFF;
    }
    .right{
        width: 27.92px;
        height: 22.33px;
    }
</style>