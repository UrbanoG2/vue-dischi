<template>

    
        <!-- <div class="genre-selection">
            <select @change="$emit('selectGenre', selectedGenre)"
                    v-model="selectedGenre"
                    name="genre" id="genre">
                <option value="all">All</option>
                <option value="rock">Rock</option>
                <option value="pop">Pop</option>
                <option value="metal">Metal</option>
                <option value="jazz">Jazz</option>
            </select>
        </div> -->

        <div class="artist-selection">
            <select @change="$emit('selectArtist', selectedArtist)"
                    v-model="selectedArtist"
                    name="artist" id="artist">
                <option value="all">All</option>
                <option value="iron maiden">Iron Maiden</option>
                <option value="metallica">Metallica</option>
                <option value="bon jovi">Bon Jovi</option>
                <option value="queen">Queen</option>
            </select>
        </div>
   

    

</template>

<script>
export default {
    name:"SearchArtist",
    props:{

    },

    data () {
        return {
            selectedArtist:"all",
        }
    }
}
</script>

<style>

</style>