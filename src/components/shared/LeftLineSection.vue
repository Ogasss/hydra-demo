<template>
    <div class="headerWrapper">
        <div class="leftPart">
            <div class="introductionTitle">
                <slot name="title"></slot>
            </div>
            <div class="to">
                <span class="introductionLittleTittle">
                    <slot name="littleTitle"></slot>
                </span>
                <img class="leftLine" :src="leftLine" alt="">
            </div>
        </div>
        <div class="sectionWrapper">
            <div class="introductionSection">
                <slot name="section"></slot>
            </div>
        </div>
    </div>
</template>

<script>
import leftLine from '../../assets/leftLine.svg'
export default {
    setup(){
        return{
            leftLine
        }
    }
}
</script>

<style scoped>
    .introductionTitle{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 700;
        font-size: 36px;
        line-height: 44px;
        color: #FFFFFF;
    }
    .introductionLittleTittle{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 300;
        font-size: 36px;
        line-height: 44px;
        color: #FFFFFF;
    }
    .introductionSection{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 400;
        font-size: 16px;
        line-height: 20px;
        color: #FFFFFF;
        opacity: 0.7;
    }
    .headerWrapper{
        display: flex;
        justify-content: space-between;
    }
    .headerWrapper .sectionWrapper{
        display: flex;
        width: 652px;
        height: 98px;
    }
    .sectionWrapper .introductionSection{
        margin: auto;
    }
    .leftPart{
        width: auto;
    }
    .leftPart .to{
        margin-top: 10px;
    }
    .leftPart .to .leftLine{
        margin-top: -50%;
        position: relative;
        top: 35px;
    }
    .to .introductionLittleTittle{
        margin-right: 30px;
    }
    .headerWrapper{
        display: flex;
        justify-content:center;
    }
    .leftPart{
        margin-right: 140px;
    }

    @media (max-width: 1520px){
        .leftPart{
            width: 50%;
        }
    }
</style>