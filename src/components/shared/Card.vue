<template>
    <div class="theCardWrapper">
        <div class="cardImageWrapper">
            <img class="cardImage" :src="src" alt="">
        </div>

        <div class="title">
            <slot></slot>
        </div>

        <div class="line"></div>

        <div class="section">
            Vitae sapien pellentesque habitant morbinunc. Viverra aliquet  porttitor rhoncus libero justo laoreet sit amet vitae.
        </div>

        <Button class="button">
            TRY IT NOW
        </Button>
    </div>
</template>

<script>
import Button from './button.vue'
export default {
    props:[
        'src'
    ],
    components:{
        Button
    },
    setup(props){
        const {src} = props
        return {
            src
        }
    }
}
</script>

<style scoped>
    .theCardWrapper{
        padding: 23px 45px;
        display: flex;
        flex-direction: column;
        align-items: center;
        width: 310px;
        height: 511px;
        background: radial-gradient(50% 50% at 50% 50%, #433D60 0%, #211E2E 100%);
        border-radius: 40px;
    }
    .cardImageWrapper{
        width: 219px;
        height: 219px;
        background: rgba(14, 14, 14, 0.32);
        display: flex;
        border-radius: 50%;
        justify-content: center;
        align-items: center;
        margin-bottom: 21px;
    }
    .theCardWrapper .title{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 700;
        font-size: 24px;
        line-height: 29px;
        color: #FFFFFF;
        margin-bottom: 17.5px;
    }
    .theCardWrapper .line{
        border: 1px solid rgba(192, 183, 232, 0.33);
        height: 1px;
        width: 154px;
        margin-bottom: 21.5px;
    }
    .theCardWrapper .section{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 400;
        font-size: 12px;
        line-height: 15px;
        color: #FFFFFF;
        margin-bottom: 35px;
    }
    .theCardWrapper .button{
        width: 154px;
        height: 48px;
    }
</style>