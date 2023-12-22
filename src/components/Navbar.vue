<script>
export default {
    name: 'Navbar',
}

</script>
<template>
    <nav class="navbar">
        <ul>
            <li><a href="/characters">Characters</a></li>
            <li><a href="/comics">Comics</a></li>
            <li><a href="/movies">Movies</a></li>
            <li><a href="/tv">Tv</a></li>
            <li><a href="/games">Games</a></li>
            <li><a href="/collectibles">collectibles</a></li>
            <li><a href="/videos">Videos</a></li>
            <li><a href="/fans">Fans</a></li>
            <li><a href="/news">News</a></li>
            <li><a href="/shop">Shop</a></li>
        </ul>
    </nav>
</template>
<style lang="scss" scoped>
.navbar {
    display: flex;
    align-items: center;

    ul {

        list-style-type: none;
        display: flex;
        gap: 1rem;




        a {
            text-decoration: none;
            color: #000;
            padding-bottom: 40px;




            &:hover {
                color: #0056b3;
                border-bottom: 5px solid #0056b3;
            }
        }
    }
}
</style>