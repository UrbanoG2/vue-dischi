<template>
    <div class="card-container">
        <div class="card-img">
            <img :src="poster" alt="">
        </div>
                    
        <div class="card-text">
            <h2>{{ title }}</h2>

            <h4>{{ author }}</h4>

            <h4>{{ year }}</h4>
        </div>
    </div>
</template>

<script>
export default {
    name:"Album",
    props:{
        poster:String,
        title:String,
        author:String,
        year:String
    }
}
</script>

<style>
    .card-img {
        overflow: hidden;             
    }

    img {
        width: 100%;
        padding: 1.5em;
    }

    h2 {
        color: white;
        text-transform: uppercase;
        text-align: center;
        font-size: 1em;
        margin-top: 3%;
    }

    h4 {
        color: grey;
        text-align: center;
        text-transform: uppercase;
        font-size: 0.8em;
    }
</style>