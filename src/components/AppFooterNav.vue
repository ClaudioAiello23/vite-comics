<!-- PARTE VUE JS-->

<script>
export default {
    name: 'AppFooterNav',
    data() {
        return {
            titleComics: 'DC COMICS',

            dcComics: [
                {
                    menuName: 'Characters',
                    link: '#',
                },
                {
                    menuName: 'Comics',
                    link: '#',
                },
                {
                    menuName: 'Movies',
                    link: '#',
                },
                {
                    menuName: 'Tv',
                    link: '#',
                },
                {
                    menuName: 'Games',
                    link: '#',
                },
                {
                    menuName: 'Videos',
                    link: '#',
                },
                {
                    menuName: 'News',
                    link: '#',
                }
            ],

            titleShop: 'SHOP',

            shops: [
                {
                    menuName: 'Shop DC',
                    link: '#',
                },
                {
                    menuName: 'Shop DC Collectibles',
                    link: '#',
                }
            ],

            titleDc: 'DC',

            dc: [
                {
                    menuName: 'Terms of Use',
                    link: '#',
                },
                {
                    menuName: 'Privacy Policy (New)',
                    link: '#',
                },
                {
                    menuName: 'Ad Choices',
                    link: '#',
                },
                {
                    menuName: 'Advertising',
                    link: '#',
                },
                {
                    menuName: 'Jobs',
                    link: '#',
                },
                {
                    menuName: 'Subscriptions',
                    link: '#',
                },
                {
                    menuName: 'Talent Workshops',
                    link: '#',
                },
                {
                    menuName: 'CPSC Certificates',
                    link: '#',
                },
                {
                    menuName: 'Ratings',
                    link: '#',
                },
                {
                    menuName: 'Shop Help',
                    link: '#',
                },
                {
                    menuName: 'Contact Us',
                    link: '#',
                }
            ],

            titleSites: 'SITES',

            sites: [
                {
                    menuName: 'DC',
                    link: '#',
                },
                {
                    menuName: 'MAD Magazine',
                    link: '#',
                },
                {
                    menuName: 'DC Kids',
                    link: '#',
                },
                {
                    menuName: 'DC Universe',
                    link: '#',
                },
                {
                    menuName: 'DC Power Visa',
                    link: '#',
                },
            ],
        }
    }
}
</script>

<!-- PARTE HTML -->
<template>
    <div class="f_box_1">
        <div class="f_nav_1">
            <h2> {{ titleComics }}</h2>
            <nav>
                <ul>
                    <li v-for="comics in dcComics">
                        <a href="#">{{ comics.menuName }}</a>
                    </li>
                </ul>
            </nav>
            <h2> {{ titleShop }}</h2>
            <nav>
                <ul>
                    <li v-for="shop in shops">
                        <a href="#">{{ shop.menuName }}</a>
                    </li>
                </ul>
            </nav>
        </div>

        <div class="f_nav_2">
            <h2> {{ titleDc }}</h2>
            <nav>
                <ul>
                    <li v-for="dc in dc">
                        <a href="#">{{ dc.menuName }}</a>
                    </li>
                </ul>
            </nav>
        </div>

        <div class="f_nav_3">
            <h2> {{ titleSites }}</h2>
            <nav>
                <ul>
                    <li v-for="site in sites">
                        <a href="#">{{ site.menuName }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </div>
</template>

<!-- PARTE SCSS-->
<style lang="scss" scoped>
.f_box_1 {
    display: flex;
    padding: 3.125rem 0;

    h2 {
        padding: 0.625rem 0;
        font-size: 1.25rem;
        color: white;
    }

    .f_nav_2 {
        padding: 0 1.875rem;

    }

    nav {
        li {
            list-style: none;
            padding: .125rem 0;

            a {
                text-decoration: none;
                color: grey;
                font-size: 0.75rem;
            }
        }
    }
}
</style>