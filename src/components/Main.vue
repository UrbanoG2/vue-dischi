<template>
    <div>
        <div class="main-container">
            <div class="cards-container">
                <div class="card">
                    <div class="card-img">
                        <img src="https://www.onstageweb.com/wp-content/uploads/2018/09/bon-jovi-new-jersey.jpg" alt="">
                    </div>

                    <div class="title-album">
                        <h2>New Jersey</h2>
                    </div>

                    <div class="artist">
                        Bon Jovi
                    </div>

                    <div class="date">
                        1988
                    </div>
                </div>

                <div class="card">

                </div>

                <div class="card">

                </div>

                <div class="card">

                </div>

                <div class="card">

                </div>

                <div class="card">

                </div>

                <div class="card">

                </div>

                <div class="card">

                </div>

                <div class="card">

                </div>

                <div class="card">

                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:"Main",
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

                .card-img {
                    overflow: hidden;
                    
                    img {
                        width: 100%;
                        padding: 1.5em;
                    }
                }

                .title-album,
                .artist,
                .date {
                    color: white;
                    text-transform: uppercase;
                    text-align: center;
                    font-size: 0.8em;
                    margin-top: 3%;
                }

                .artist,
                .date {
                    color: grey;
                }
            }
        }
    }
</style>