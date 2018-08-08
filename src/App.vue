<template>
  <div id="app">
    <project-grid></project-grid>
  </div>
</template>

<script>
import projectGrid from "./components/ProjectGrid.vue";

export default {
  name: "app",
  components: {
    projectGrid
  }
};
</script>

<style>
@import url("https://fonts.googleapis.com/css?family=Roboto+Slab|Roboto:900|Work+Sans:200");
body {
  margin: 0px 5%;
}
</style>
