<script>
import CardsList from "../assets/data/dc-comics.json"
import CardBox from "./CardBox.vue"
  export default {
    name: "CardContainer",
    data (){
        return {
          CardsList,  
        }
    },
    components: {
        CardBox,
    }
  }
</script>

<template>
    <div class="card_container">
        <CardBox class="card bg-dark" v-for="item in CardsList" :img="item.thumb" :title="item.series"></CardBox>
    </div>
</template>