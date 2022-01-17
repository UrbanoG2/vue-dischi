<template>
    <div>
        <div class="header-container">
            <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/1/19/Spotify_logo_without_text.svg/2048px-Spotify_logo_without_text.svg.png" alt="">
        </div>
    </div>
</template>

<script>
export default {
    name:"Header",
}
</script>

<style lang="scss" scoped>

    .header-container {
        width: 100%;
        background-color:  #2E3A46;

        img {
            width: 7%;
            padding: 1em;
        }
    }
</style>