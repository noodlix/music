<template>
    <div class="likedSongs">
        <div class="oneSong">
            <div class="songPicture"></div>
            <div class="textSong">
                <div class="titleSong">Song Title</div>
                <div class="artistSong">The artist</div>
            </div>
        </div>
        <div class="oneSong">
            <div class="songPicture"></div>
            <div class="textSong">
                <div class="titleSong">Song Title</div>
                <div class="artistSong">The artit</div>
            </div>
        </div>
    </div>
</template>
<script>
// import Vue from 'vue'
// import Spotify from 'spotify-web-api-node'
// import VueSpotify from 'vue-spotify'

// Vue.use(VueSpotify, new Spotify())
// Vue.spotify.getUser('petteralexis')
//    .then(function(data) {
//        console.log('Some information about this user', data.body);
//    }, function(err) {
//        console.log('Something went wrong!', err);
//    })


// this.spotify.getUser('petteralexis')
//     .then(function(data) {
//         console.log('Some information about this user', data.body);
//     }, function(err) {
//         console.log('Something went wrong!', err);
//     })
import SpotifyWebApi from 'spotify-web-api-js';

const spotifyApi = new SpotifyWebApi();
spotifyApi.setClientId('983d115640d6422e8f4b79b86a55de75');



export default {
    name: 'liked-songs',
    data() {
        return {
            isPlaying: false,
            liked: none,
        }
    },
    emits: [],
    methods: {
        beforeMount() {
            spotifyApi.play({ uris: ['spotify:track:4uLU6hMCjMI75M1A2tKUQC'] })
                .then(() => {
                    this.handlePlaybackStarted();
                    this.isPlaying = true;
                })
                .catch((error) => {
                    console.error('Failed to start playing music:', error);
                });
        },
        handlePlaybackStarted() {}
    }
}
</script>
<style lang="scss">
.likedSongs {
    width: 100%;
    padding-left: 30px;

    .oneSong {
        display: flex;
        flex-direction: row;
        gap: 20px;
        margin-top: 20px;
    }
}

.songPicture {
    width: 100px;
    height: 100px;
    background-color: rgb(255, 255, 255);
    box-shadow: 5px 5px 5px rgb(101, 88, 155);

}

.titleSong {
    font-weight: 700;
    font-size: 30px;
    color: white;
}

.artistSong {
    font-weight: 400;
    font-size: 20px;
    color: white;
}
</style>