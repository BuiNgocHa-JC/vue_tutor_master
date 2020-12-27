<template>
  <div id="app">
    <action v-bind:message="messageAction"></action>
    <grid v-bind:photos="photos"></grid>
  </div>
</template>
<script>
  import action from './components/action'
  import grid from './components/grid'
  export default {
    name: 'App',
    components: { action, grid },
    data: function () {
      return {
        photos: [
          {
            id: 0,
            url: "https://i.imgur.com/p3IKY9G.jpg"
          }
        ],
        messageAction: "It's working !"
      }
    }
  }
</script>
<style>
  * {
    box-sizing: border-box;
  }
  body {
    margin: 0;
    font-family: Arial;
  }
</style>