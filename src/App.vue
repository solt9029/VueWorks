<template>
  <div id="app">
    <app-header></app-header>
    <cards></cards>
    <app-footer></app-footer>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader'
import Cards from "./components/Cards"
import AppFooter from "./components/AppFooter"
import Minigrid from "minigrid"
import "bootstrap/dist/css/bootstrap.min.css"
require("bootstrap")
import "material-design-lite/dist/material.indigo-pink.min.css"
require("material-design-lite")
import "font-awesome/css/font-awesome.min.css"

let grid
function init() {
  grid = new Minigrid({
    container: '.cards',
    item: '.card',
    gutter: 12
  })
  grid.mount()
}
function update() {
  grid.mount()
}

document.addEventListener('DOMContentLoaded', init)
window.addEventListener('resize', update)

export default {
  name: 'app',
  components:{AppHeader,Cards,AppFooter}
}
</script>

<style>
</style>