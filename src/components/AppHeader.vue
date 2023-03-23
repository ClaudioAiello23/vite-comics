<!-- PARTE VUE JS-->
<script>
export default {
    data() {
        return {
            name: 'AppHeader',
            headerMenu: [
                {
                    menuName: 'CHARACTERS'

                },
                {
                    menuName: 'COMICS'

                },
                {
                    menuName: 'MOVIES'

                },
                {
                    menuName: 'TV'

                },
                {
                    menuName: 'GAMES'

                },
                {
                    menuName: 'COLLECTIBLES'

                },
                {
                    menuName: 'VIDEOS'

                },
                {
                    menuName: 'FANS'

                },
                {
                    menuName: 'NEWS'

                },
                {
                    menuName: 'SHOP'

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
            <li>{{ headerMenu[0].menuName }}</li>
        </ul>
    </nav>
</template>

<!-- PARTE SCSS-->
<style lang="scss" scoped></style>