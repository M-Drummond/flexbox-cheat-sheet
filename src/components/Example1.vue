<template>
    <div class="Example" id="Example1">

        <div class="container limited-width">
            <h2>Header layout</h2>
        </div>

        <!-- header navigation often shows this pattern -->

        <div class="three-elements container limited-width">

            <div class="toggle-button" aria-label="navigation toggle button">
                <button aria-label="show/hide navigation"><bars/></button>
            </div>

            <div class="logo" aria-label="example logo">
                Logo or Heading
            </div>

            <div class="search">
                Search Box
            </div>

        </div>


    </div>

</template>

<script setup lang="ts">
    
    import bars from './icons/bars.vue';

</script>


<style scoped>
 

.three-elements.container {
    justify-content: start;
    width: 100%;
    flex-direction: row;
    background: #eee;
    padding: 2rem 1.5rem;
}

.three-elements.container > div {
    margin-bottom: 1.25rem
}

.search {display: none;}

.three-elements.container .toggle-button  {
    padding-right: 1.25rem;
    flex-basis: 50px;
}
 

@media only screen and (min-width: 767px) {
    .three-elements.container {
        justify-content: space-between;
        align-items: center;
        width: 100%;
        
    }

    .three-elements.container>div {
        margin-bottom: 0;
    }

    .search {display: block;}

}
</style>