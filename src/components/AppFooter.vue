<template>
  <footer class="container-fluid">
    <small><a href="http://solt9029.com" class="copyright">Copyright (C) Kenshi Shiode.</a></small>
  </footer>
</template>

<script>
export default {
  name: 'app-footer'
}
</script>

<style scoped>
.copyright{
  color:#fff;
}
.copyright:hover{
  color:#ddd;
  text-decoration:none;
}
footer {
  text-align: center;
  padding: 10px;
  background:linear-gradient(45deg,rgba(150,50,150,0.9), rgba(10,180,150,0.9));
}
</style>