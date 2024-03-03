<template>

    <div>

        <div class="container limited-width">
            <h2>Form Layout, labels above / below</h2>
        </div>


        <div class="Example-1 container limited-width">
            <form>
                <label for="fname">
                    <span>First name:</span>
                    <input type="text" id="fname" name="fname">

                </label>
                <label for="lname">
                    <span>Last name:</span>
                    <input type="text" id="lname" name="lname">

                </label>
                <button aria-label="submit form">Submit</button>
            </form>

        </div>

    </div>
</template>

<style scoped>

.Example {
    margin: 2rem auto;
    width: 100%;
    background: #eee ;
}

form {
    display: flex;
    flex-direction: column ;
    width: 100%;
    align-items: start ;
}

form label {
    width: 100%;
    display: flex;
    flex-direction: column;
    margin-bottom: 1rem;
    justify-content: start ;
    align-items: start ;
}

@media only screen and ( min-width : 767px )  {
    form label {
        flex-direction: row ;
        align-items: baseline;
    }
    
}

form label span {
    display: block;
    margin-right: .5rem;
    margin-bottom: 1rem ;
    max-width: 100%;
}

@media only screen and ( min-width : 440px ) {
    form label span {
        min-width: 125px;
    }
}

@media only screen and ( min-width : 960px ) {
    form label span {
        margin-bottom: 0;
    }
}

form label input {
    width: 100%;
    padding: .5rem ;
    box-sizing: border-box ;
}

form label input:focus {
    outline: 1px solid #666;
    border-radius: 4px;
}

form button {
    width: 100%;
    padding: .5rem;
    transition: .125s ease-in all ;
}

form button:focus {
    outline: 1px solid #666;
    border-radius: 4px;
}

form button:hover {
    color: #fff;
    background-color: #000;
    text-decoration: underline ;
}




</style>