<template>
<div class="demo-card-square mdl-card mdl-shadow--2dp card">
  <div 
    class="mdl-card__title mdl-card--expand" 
    :style="{ background: `url('${urlImage}') no-repeat`, backgroundSize:'320px 240px' }">
    <h2 class="mdl-card__title-text">{{ titleText }}</h2>
  </div>
  <div class="mdl-card__actions mdl-card--border">
    <a 
      target="_blank" 
      :href="urlPage" 
      class="mdl-button mdl-button--colored mdl-js-button mdl-js-ripple-effect">
      <i class="fa fa-external-link icon"></i>
      Find Out More
    </a>
  </div>
</div>
</template>

<script>
export default {
  name: 'card',
  props:{
    titleText:{
      type: String,
      required: true
    },
    urlImage:{
      type: String,
      required: true
    },
    urlPage:{
      type: String,
      required: true
    }
  }
}
</script>

<style scoped>
*{
  word-break:break-all;/* 文字列の折り返し */
}
.demo-card-square.mdl-card{
  width:320px;
}
.demo-card-square>.mdl-card__title{
  color:#fff;
  height:240px;
}
.mdl-card__title-text{
  -webkit-text-stroke:1.5px black;
  font-weight:900;
  font-size:2em;
}
.mdl-card__actions{
  text-align:center;
}
.icon{
  margin-right:10px;
}
</style>