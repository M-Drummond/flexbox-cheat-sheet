<template>
    <div class="Example container limited-width">
        <div class="grid-container">

            <div>
                <img src="https://placehold.co/600x400/EEE/31343C" alt="image for the grid" />
            </div>

            <div>
                <img src="https://placehold.co/600x400/EEE/31343C" alt="image for the grid" />
            </div>
            <div>
                <img src="https://placehold.co/600x400/EEE/31343C" alt="image for the grid" />
            </div>
            <div>
                <img src="https://placehold.co/600x400/EEE/31343C" alt="image for the grid" />
            </div>
            <div>
                <img src="https://placehold.co/600x400/EEE/31343C" alt="image for the grid" />
            </div>
            <div>
                <img src="https://placehold.co/600x400/EEE/31343C" alt="image for the grid" />
            </div>
            <div>
                <img src="https://placehold.co/600x400/EEE/31343C" alt="image for the grid" />
            </div>
            <div>
                <img src="https://placehold.co/600x400/EEE/31343C" alt="image for the grid" />
            </div>
 

        </div>
    </div>
</template>

<style scoped>

.grid-container {
    display: grid;
    grid-template-columns: repeat(2, minmax(0, 1fr));
    gap: 1rem;
}


/* medium screens */

@media only screen and (min-width: 767px) {
    .grid-container {;
        grid-template-columns: repeat(4, minmax(0, 1fr));
    }
}

/* larger screens  */

@media only screen and (min-width: 1200px) {
    .grid-container {
        grid-template-columns: repeat(8, minmax(0, 1fr));
    }
}

.grid-container img {
    max-width: 100%;
    height: auto;
    border: 1px solid #ccc;
}

</style>