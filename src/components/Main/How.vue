<template>
    <div class="theHowWrapper">
        <LeftLineSection>
            <template v-slot:title>
                HOW WE BUILD
            </template>
            <template v-slot:littleTitle>
                WITH HYDRA VR?
            </template>
            <template v-slot:section>
                Vitae sapien pellentesque habitant morbi tristique senectus et netus et. Feugiat nibh sed pulvinar proin gravida hendrerit lectus. Mi sit amet mauris commodo quis imperdiet massa tincidunt nunc. Viverra aliquet eget sit amet tellus. Ornare lectus sit amet est placerat in. Lectus magna fringilla urna porttitor rhoncus vitae.
            </template>
        </LeftLineSection>
        <div class="ballsWrapper">
            <BallItem>
                <template v-slot:number>
                    <div class="ballNumber">01</div>
                </template>
                <template v-slot:text>
                    3D Conception <br>& Design
                </template>
            </BallItem>

            <BallItem>
                <template v-slot:number>
                    <div class="ballNumber">02</div>
                </template>
                <template v-slot:text>
                    Interaction<br>Design
                </template>
            </BallItem>

            <BallItem>
                <template v-slot:number>
                    <div class="ballNumber">03</div>
                </template>
                <template v-slot:text>
                    VR World<br>User Testing
                </template>
            </BallItem>

            <BallItem>
                <template v-slot:number>
                    <div class="ballNumber">04</div>
                </template>
                <template v-slot:text>
                    Hydra VR<br>Deploy
                </template>
            </BallItem>
        </div>
        <img class="Vector15" :src="Vector15" alt="">
    </div>
</template>

<script>
import Vector15 from '../../assets/Vector15.svg'

import LeftLineSection from '../shared/LeftLineSection.vue'
import BallItem from '../shared/BallItem.vue'

export default {
    components:{
        LeftLineSection,
        BallItem
    },
    setup(){
        return{
            Vector15
        }
    }
}
</script>

<style scoped>
    .theHowWrapper{
        margin-top: 123px;
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        margin-bottom: 138px;
    }
    .ballsWrapper{
        width: 1440px;
        margin-top: 143px;
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
    .ballNumber{
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 700;
        font-size: 64px;
        line-height: 78px;
        color: #343045;
    }
    .Vector15{
        width: 100%;
        margin-top: 130px;
        position: absolute;
        z-index: -1;
    }
</style>