<template>
    <vue-typer text='Hello World! I was registered locally!'></vue-typer>
</template>

<script>
import { VueTyper } from 'vue-typer';
var VueTyper = require('vue-typer').VueTyper

var myComponent = {
    components: {
        VueTyper,
        'vue-typer': VueTyper
    }
}
export default {
    name: "Typer"
}
</script>

<style>

</style>

