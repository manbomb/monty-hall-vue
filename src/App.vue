<template>
    <div id="app">
        <h1>Problema de Monty Hall</h1>
        <Door number="1" :hasGift="true" />
    </div>
</template>

<script>
import Door from './components/Door'

export default {
    name: 'App',
    components: {
        Door
    },
    data: function() {
        return {
            started: false
        }
    }
}
</script>

<style>

* {
    box-sizing: border-box;
    font-family: 'Montserrat', sans-serif;
}

body {
    color: white;
    background: #355C7D;  /* fallback for old browsers */
    background: -webkit-linear-gradient(to right, #C06C84, #6C5B7B, #355C7D);  /* Chrome 10-25, Safari 5.1-6 */
    background: linear-gradient(to right, #C06C84, #6C5B7B, #355C7D); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
}

#app {
    display: flex;
    flex-direction: column;
    align-items: center;
}

#app h1 {
    border: 1px solid #000;
    background-color: #0004;
    padding: 20px;
    margin-bottom: 60px;
}

</style>