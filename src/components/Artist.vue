<template lang="pug">
  li.artist
    h2: a(:href="artist.url" target="_blank") {{ artist.name }}
    img(:src="artist.image[2]['#text']")

</template>

<script>

export default {
  name: 'artist',
  props: [ 'artist' ]
}  
  
</script>

<style>
li{
	display: inline-block;
  	margin: 10px;
  	border: 5px solid #41B883;
  	border-radius: 13px;
}
</style>
