<template>
    <div class="row row-cols-1 row-cols-sm-4 mx-auto my-4">
        <Album v-for="album in albumJson" :key="album.album" :albumName="album.album" :year="album.date" :artist="album.artist" :cover="album.cover" />
    </div>
</template>

<script setup>
    import Album from '../components/Album.vue'
</script>

<script>
// https://gist.github.com/dimayakovlev/ffbe59c73393d254fd66fd29dffc97e5
import data from "../assets/data/beatlesalbums.json";

export default{
          data(){
              return{
                  albumJson: data
              }
          }
      };
</script>