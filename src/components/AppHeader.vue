<template>
  <header class="jumbotron" id="jumbotron">
    <div class="container">
      <h1>Works @solt9029</h1>
      <p>This page is for introduction of many programming works I have ever created. I'm very interested in PHP and web applications. Also, I like to use hardware such as 3D printer and electronic parts to make something interesting. Thank you!</p>
    </div>
  </header> 
</template>

<script>
export default {
  name: 'app-header'
}
</script>

<style scoped>
header.jumbotron {
  background:linear-gradient(45deg, rgba(150,50,150,0.9), rgba(10,180,150,0.9)), url("/static/img/header.png");
  background-color:#000;
  background-position: center center;
  background-size: cover;
  color: #fff;
}
.title{
  color:#fff;
  text-decoration:none;
}
.title:hover{
  color:#ddd;
  text-decoration:none;
}
</style>