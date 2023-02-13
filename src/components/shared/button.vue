<template>
    <div>
        <button :class="buttonStyle">
            <slot/>
        </button>
    </div>
</template>

<script>
import { computed } from 'vue'
export default {
    props:[
        'simple',
        'ball'
    ],
    setup(props){
        const { simple,ball } = props
        const buttonStyle = computed(()=>{
            let style
            if(simple === ''){
                style = 'hydraButtonSimple'
            }else{
                style = 'hydraButton'
            }
            if(ball === ''){
                style = style + ' ball'
            }
            return style
        })
        return {
            buttonStyle
        }
    }
}
</script>

<style scoped>
    .hydraButtonSimple{
        border: 2px solid #FFF;
        width: 100%;
        height: 100%;
        border-radius: 40px;
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 700;
        font-size: 12px;
        line-height: 15px;
        color: #FFFFFF;
        display: flex;
        justify-content: center;
        align-items: center;
        transition: all ease 0.3s;
    }
    .hydraButtonSimple:hover{
        background: linear-gradient(145deg, #303030, #202020);
    }
    .hydraButtonSimple:active{
        background: none;
    }
    
    .hydraButton{
        background: linear-gradient(90deg, #8176AF 0%, #C0B7E8 100%);
        width: 100%;
        height: 100%;
        border-radius: 40px;
        font-family: 'Montserrat';
        font-style: normal;
        font-weight: 700;
        font-size: 12px;
        line-height: 15px;
        color: #343045;
        opacity: 0.9;
    }
    .hydraButton:hover{
        opacity: 1;
    }
    .hydraButton:active{
        opacity: 0.9;
    }
    .ball{
        border-radius: 50%;
        opacity: 1;
    }
</style>