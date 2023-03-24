<!-- PARTE VUE JS-->

<script>
export default {
    name: 'AppHeaderNav',
    data() {
        return {
            headerMenu: [
                {
                    menuName: 'CHARACTERS',
                    link: '#',
                    target: '_self',
                },
                {
                    menuName: 'COMICS',
                    link: '#',
                    target: '_self',
                },
                {
                    menuName: 'MOVIES',
                    link: '#',
                    target: '_self',
                },
                {
                    menuName: 'TV',
                    link: '#',
                    target: '_self',
                },
                {
                    menuName: 'GAMES',
                    link: '#',
                    target: '_self',
                },
                {
                    menuName: 'COLLECTIBLES',
                    link: '#',
                    target: '_self',
                },
                {
                    menuName: 'VIDEOS',
                    link: '#',
                    target: '_self',
                },
                {
                    menuName: 'FANS',
                    link: '#',
                    target: '_self',
                },
                {
                    menuName: 'NEWS',
                    link: '#',
                    target: '_self',
                },
                {
                    menuName: 'SHOP',
                    link: '#',
                    target: '_self',
                },
            ]
        }
    }
}
</script>

<!-- PARTE HTML -->
<template>
    <nav>
        <ul>
            <li v-for="h_nav in headerMenu">
                <a href="#">{{ h_nav.menuName }}</a>
            </li>
        </ul>
    </nav>
</template>

<!-- PARTE SCSS-->
<style lang="scss" scoped>
nav {

    li {
        list-style: none;
        display: inline-block;
        padding: 0 .75rem;

        a {
            text-decoration: none;
            color: black;
            font-weight: bold;
            font-size: 0.75rem;
        }
    }
}
</style>