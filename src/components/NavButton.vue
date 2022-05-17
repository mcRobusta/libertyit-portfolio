<template>
    <vs-button :color="colour" type="line" line-origin="left" size="large" style="width: 190px; text-align: left">
        <b>{{heading}}</b>
    </vs-button>
</template>

<script>
export default {
    name:'NavButton',
    props: {
        heading: String,
        colour: String,
        route: String
    }
}
</script>

<style scoped>
vs-button {
    font-family: 'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
}
</style>