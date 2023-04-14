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

<style lang="scss" scoped>
@use "../assets/scss/partials/variables" as *;
.card_container{
  display: flex;
  justify-content: center;
  align-items: center;
  flex-wrap: wrap;
}
.card{
    width: calc(100% / 6);
    aspect-ratio: 1/1;
    border: none;
}
</style>