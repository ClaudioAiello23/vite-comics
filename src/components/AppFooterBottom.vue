<!-- PARTE VUE JS-->

<script>
export default {
    name: 'AppFooterBottom',
    data() {
        return {

        }
    }
}
</script>

<!-- PARTE HTML -->
<template>
    <div class="footer_bottom_container">
        <div><button>A</button></div>
        <div>
            <div>FOLLOWUS</div>
            <div>
                <ul>
                    <li><a href="#">CBEFG</a></li>
                </ul>
            </div>
        </div>
    </div>
</template>

<!-- PARTE SCSS-->
<style lang="scss" scoped>
.footer_bottom_container {
    background-color: #303030;
    padding: 1.875rem;
    display: flex;
    justify-content: space-between;
}
</style>