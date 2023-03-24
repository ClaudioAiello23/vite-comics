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
    <div class="f_box_2">
        <div><button type="button">SIGN-UP NOW!</button></div>
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
.f_box_2 {
    padding: 1.875rem 0;
    display: flex;
    justify-content: space-between;

    button {
        background-color: #303030;
        color: white;
        padding: .9375rem;
        border: 2px solid #0282f9;
        cursor: pointer;
    }
}
</style>