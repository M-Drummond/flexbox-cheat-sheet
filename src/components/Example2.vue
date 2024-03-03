<template>
    <div class="Example" id="Example2">

        <div class="container limited-width">
            <h2>Header layout 2 - Two Items, left align</h2>
        </div>

        <!-- header navigation often shows this pattern -->

        <div class="two-elements container limited-width">

            <div class="toggle-button" aria-label="navigation toggle button">
                <button aria-label="show/hide navigation">
                    <bars />
                </button>
            </div>

            <div class="logo" aria-label="example logo">
                Logo or Heading
            </div>



        </div>


    </div>

</template>

<script setup lang="ts">
import bars from './icons/bars.vue';
</script>

<style scoped>
 
.two-elements.container {
    justify-content: start;
    width: 100%;
    flex-direction: row;
    background: #eee;
    padding: 2rem 1.5rem;
}

.two-elements.container>div {
    margin-bottom: 1.25rem
}

.two-elements.container .toggle-button {
    padding-right: 1.25rem;
    flex-basis: 50px;
}

@media only screen and (min-width: 767px) {
    .two-elements.container {
        justify-content: start;
        align-items: center;
        width: 100%;
        flex-direction: row;
    }

    .two-elements.container>div {
        margin-bottom: 0;
    }



}
</style>