<script>
import jumbotron from './jumbotron.vue';
export default {
    name: 'AppMain',
    components: {
        jumbotron,
    },
    data() {
        return {
            items: [
                {
                    "thumb": "https://www.coverbrowser.com/image/action-comics/1-1.jpg",
                    "price": "$19.99",
                    "series": "Action Comics",
                    "type": "comic book",
                },
                {
                    "thumb": "https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg",
                    "price": "$3.99",
                    "series": "American Vampire 1976",
                    "type": "comic book",
                },
                {
                    "thumb": "https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg",
                    "price": "$16.99",
                    "series": "Aquaman",
                    "type": "graphic novel",
                },
                {
                    "thumb": "https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg",
                    "price": "$2.99",
                    "series": "Batgirl",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg",
                    "price": "$3.99",
                    "series": "Batman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg",
                    "price": "$2.99",
                    "series": "Batman Beyond",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg",
                    "price": "$3.99",
                    "series": "Batman/Superman",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg",
                    "price": "$4.99",
                    "series": "Batman/Superman Annual",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg",
                    "price": "$5.99",
                    "series": "Batman: The Joker War Zone",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg",
                    "price": "$6.99",
                    "series": "Batman: Three Jokers",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg",
                    "price": "$4.99",
                    "series": "Batman: White Knight Presents: Harley Quinn",
                    "type": "comic book",
                },
                {
                    "thumb": "https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg",
                    "price": "$16.99",
                    "series": "Catwoman",
                    "type": "graphic novel",
                },
            ]



        }
    }

}

</script>
<template>
    <div class="container-main">
        <jumbotron />

        <div class="current-series">
            <h2>CURRENT SERIES</h2>
            <div class="container-items">
                <div v-for="item in items" :key="item.series" class="item">
                    <img :src="item.thumb" :alt="item.series" class="item-thumb">
                    <div class="item-info">
                        <h5>{{ item.series }}</h5>
                        <h6>{{ item.type }}</h6>
                        <button class="buy-button">BUY - {{ item.price }}</button>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<!-- <style lang="scss" scoped>
.container-item {
    width: 100%;
    padding-top: 50px;
    background-color: #1c1c1c;
}
</style> -->

<style lang="scss" scoped>
.container-main {
    position: relative;
}

.current-series {

    padding: 20px;
    text-align: center;
    background-color: #1c1c1c;

    h2 {
        width: 270px;
        display: flex;
        justify-content: start;
        margin-left: 245px;
        background-color: #007bff;
        position: absolute;
        top: 32%;
        color: white;
    }


    .container-items {
        width: 80%;
        margin: auto;
        display: flex;
        flex-wrap: wrap;
        justify-content: center;
        gap: 20px;
        padding-top: 50px;
    }

    .item {
        width: calc((100% / 7));
        margin-bottom: 20px;
        display: flex;
        flex-direction: column;
        justify-content: space-between;
    }

    .item-thumb {
        width: 100%;
        height: 300px;
    }

    .item-info {
        padding: 10px;

        h5 {
            margin: 10px 0 5px;
            font-size: 14px;
            color: white;
        }

        h6 {
            margin: 0;
            font-size: 12px;
            color: #555;
        }

        .buy-button {
            background-color: #007bff;
            color: white;
            border: none;
            padding: 10px;
            width: 100%;
            border-radius: 5px;
            margin-top: 10px;
            cursor: pointer;

            &:hover {
                background-color: #0056b3;
            }
        }
    }






}
</style>
