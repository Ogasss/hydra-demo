<template>
    <div class="theTechnologiesWrapper">
        <img class="TechnologiesBackImage" :src="TechnologiesBackImage" alt="">
        <div class="contentWrapper">
            <div class="title">TECHNOLOGIES & HARDWARE</div>
            <div class="littleTittle">USED BY HYDRA VR.</div>
            <div class="buttonWrapper">
                <Button class="button"><img :src="down" alt=""></Button>
            </div>
        </div>
        <div class="iconsWrapper">
            <img :src="UNREAL" alt="">
            <img :src="Unity" alt="">
            <img :src="oculus" alt="">
            <img :src="VIVE" alt="">
        </div>
    </div>
</template>

<script>
import TechnologiesBackImage from '../../assets/TechnologiesBackImage.svg'
import down from '../../assets/down.svg'
import UNREAL from '../../assets/UNREAL.svg'
import Unity from '../../assets/Unity.svg'
import oculus from '../../assets/oculus.svg'
import VIVE from '../../assets/VIVE.svg'

import Button from '../shared/button.vue'
export default {
    components:{
        Button
    },
    setup(){
        return{
            TechnologiesBackImage,
            down,
            UNREAL,
            Unity,
            oculus,
            VIVE
        }
    }
}
</script>

<style scoped>
    .theTechnologiesWrapper{
        margin-top: 114px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
    }
    .TechnologiesBackImage{
        height: 320px;
    }
    .theTechnologiesWrapper .contentWrapper{
        display: flex;
        flex-direction: column;
        align-items: center;
        margin-top: -220px;
    }
    .contentWrapper .button{
        width: 70px;
        height: 70px;
    }
    .contentWrapper .buttonWrapper{
        width: 100px;
        height: 100px;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 50%;
        background: rgba(14, 14, 14, 0.32);
    }
    .contentWrapper .title{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 700;
        font-size: 36px;
        line-height: 44px;
        color: #FFFFFF;
        margin-bottom: 11px;
    }
    .contentWrapper .littleTittle{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 300;
        font-size: 36px;
        line-height: 44px;
        color: #FFFFFF;
        margin-bottom: 61px;
    }
    .iconsWrapper{
        width: 1278px;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
</style>