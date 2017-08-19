<template>
  <div class="cards">
    <card 
      v-for="card in cards" 
      :titleText="card.titleText" 
      :urlImage="card.urlImage" 
      :urlPage="card.urlPage">
    </card>
  </div>
</template>

<script>
import Card from "./Card"
import Data from "../data/Data.json"
export default {
  name: 'cards',
  components:{
    Card
  },
  data(){
    return {
      cards: Data
    }
  }
}
</script>

<style scoped>
.cards {
  width: 100%;
  margin-top:20px;
  margin-bottom:20px;
  margin-right:auto;
  margin-left:auto;
}
</style>