<template>
    <div class="theWhyWrapper">
        <LeftLineSection>
            <template v-slot:title>
                WHY BUILD
            </template>
            <template v-slot:littleTitle>
                WITH HYDRA?
            </template>
            <template v-slot:section>
                Vitae sapien pellentesque habitant morbi tristique senectus et netus et. Feugiat nibh sed pulvinar proin gravida hendrerit lectus. Mi sit amet mauris commodo quis imperdiet massa tincidunt nunc. Viverra aliquet eget sit amet tellus. Ornare lectus sit amet est placerat in. Lectus magna fringilla urna porttitor rhoncus vitae.
            </template>
        </LeftLineSection>

        <div class="cardsWrapper">
            <img class="Vector14" :src="Vector14" alt="">
            <Card :src="CardImageOne" class="card">SIMULATION</Card>
            
            <Card :src="CardImageTwo" class="card">EDUCATION</Card>
            
            <Card :src="CardImageThree" class="card">SELF-CARE</Card>

            <Card :src="CardImageFour" class="card">OUTDOOR</Card>
        </div>

        
    </div>
</template>

<script>
import LeftLineSection from '../shared/LeftLineSection.vue'
import Card from '../shared/Card.vue'

import CardImageOne from '../../assets/CardImageOne.svg'
import CardImageTwo from '../../assets/CardImageTwo.svg'
import CardImageThree from '../../assets/CardImageThree.svg'
import CardImageFour from '../../assets/CardImageFour.svg'
import Vector14 from '../../assets/Vector14.svg'

export default {
    components:{
        LeftLineSection,
        Card
    },
    setup() {
        return {
            CardImageOne,
            CardImageTwo,
            CardImageThree,
            CardImageFour,
            Vector14
        }  
    }
}
</script>

<style scoped>
    .cardsWrapper{
        margin-top: 105px;
        display: flex;
        justify-content: center;
    }
    .cardsWrapper .card{
        margin-left: 11px;
    }
    .Vector14{
        position: absolute;
        z-index: -1;
    }
</style>