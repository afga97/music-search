<template>
  <div id="app">
    <!-- <div class="artis">
        <h2> <a v-bind:href="artist.url" target="_blank">{{ artist.name }}</a></h2>
    </div> -->
    <li class="artist"> <h2> <a v-bind:href="artist.url" target="_blank">{{ artist.name }}</a></h2> 
        <img v-bind:src="artist.image[2]['#text']">
    </li>
  </div>
</template>

<script>
export default {
    name: "artist",
    props : ['artist']
}
</script>
<style lang="stylus" scoped>
    li.artist
        display: inline
        width: 220px
    
</style>



