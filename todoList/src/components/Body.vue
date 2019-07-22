<template>
    <div>
        <InputBar></InputBar>
        <ListContainer></ListContainer>
    </div>
</template>

<script>
import InputBar from './InputBar'
import ListContainer from './ListContainer'


export default {
    data(){
        return{
            
        }
    },
    methods:{
        returnList(val){
            const item= {
                val,
                finished:false,
            }
            this.$emit("push",item);
        }
    },
    components:{
        InputBar,
        ListContainer
    }
}
</script>

<style>

</style>

