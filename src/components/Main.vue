<template>
    <div>
        <div class="main-container">
            <div class="cards-container">
                <Album class="card"
                    v-for="(album, index) in thumbs"
                    :key="index"
                    :poster="album.poster"
                    :title="album.title"
                    :author="album.author"
                    :year="album.year">
                        <!-- <div class="card-img">
                        <img :src="album.poster" alt="">
                    </div>
                    
                    <div class="card-text">
                        <h2>{{ album.title }}</h2>

                        <h4>{{ album.author }}</h4>

                        <h4>1988</h4>
                    </div> -->
                    
                </Album>

            </div>
        </div>
    </div>
</template>

<script>

import axios from "axios";
import Album from "./Album.vue"

export default {
    name:"Main",
    components : {
        Album,
    },

    data (){
        return {
            thumbs: null
        }
    },

    mounted () {
        axios
        .get ("https://flynn.boolean.careers/exercises/api/array/music")
        .then((response)=>{
            this.thumbs = response.data.response;
            console.log(this.thumbs);

        }).catch ((error)=>{
            console.log(error);
        })
    }
}
</script>

<style lang="scss" scoped>
    .main-container {
        background-color: #1E2D3B;
        display: flex;
        align-items: center;

        .cards-container {
            width: 70%;
            margin: auto;
            margin-top: 10px;
            display: flex;
            justify-content:space-between;
            flex-wrap: wrap;
            gap: 2%;

            .card {
                width: calc(100% / 5 - 20px);
                margin: 2% 0; 
                height: 300px;
                background-color:  #2E3A46;

                // .card-img {
                //     overflow: hidden;
                    
                //     img {
                //         width: 100%;
                //         padding: 1.5em;
                //     }
                // }

                // h2 {
                //     color: white;
                //     text-transform: uppercase;
                //     text-align: center;
                //     font-size: 1em;
                //     margin-top: 3%;
                // }

                // h4,
                // h4 {
                //     color: grey;
                //     text-align: center;
                //     text-transform: uppercase;
                //     font-size: 0.8em;
                // }
            }
        }
    }
</style>