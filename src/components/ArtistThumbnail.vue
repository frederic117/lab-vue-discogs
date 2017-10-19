<template>
  <div class="thumbnail" v-if="artist">
<img :src="artist.thumb" alt="" v-if="artist.thumb">
<router-link to="'artists/' + artist.id.toString()">
<h2>{{artist.title}}</h2>
</router-link>
  </div>
</template>

<script>
export default {
  name: 'ArtistThumbnail',
  props:{
    artist: Object
  }
}
 
</script>


