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
        </ul>
    </nav>
</template>
<style lang="scss" scoped>
.navbar {
    ul {
        padding: 0;
        list-style-type: none;
        display: flex;
        gap: 1rem;

        li {}

        a {
            text-decoration: none;
            color: #000;

            &:hover {
                color: #0056b3;
            }
        }
    }
}
</style>