<template>
    <div data-tilt>
        <img :src="cover || 'https://media.tenor.com/LeTLUqI-IzgAAAAd/the-beatles.gif'" style="aspect-ratio: 1 / 1; width: 300px;" />
        <h5 class="text-center">{{ albumName }} - {{ artist }}</h5>
        <p class="text-center">{{ year }}</p>
    </div>
</template>


<script>

export default{
    data(){
        return{
            albumName: 'Unknown',
            year: 'Unknown',
            artist: 'Unknown',
            cover: null
            }
        },
        props: {
            albumName: String,
            year: String,
            artist: String,
            cover: String
        },
    created(){
        this.albumName = this.$props.albumName;
        this.year = this.$props.year;
        this.artist = this.$props.artist;
        this.cover = this.$props.cover;
    }
}
</script>