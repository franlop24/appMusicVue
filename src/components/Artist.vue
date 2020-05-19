<template lang="pug">
    li.artist
        h2: a(:href="artist.url" target="_blank") {{ artist.name }}
        img(:src="artist.image[2]['#text']")
</template>

<script>
export default {
    name: 'artist',
    props: ['artist']   
}
</script>

<style lang="stylus" escoped>
    li.artist 
        display inline-block
        margin 20px
</style>