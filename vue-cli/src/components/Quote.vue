<template>
    <div>
        <div class="title">
            <slot name="title"></slot>
            <span style="color: green;"><slot name="subtitle">This's a subtitle</slot></span>
        </div>
        <hr>
        <div>
            <slot></slot>
        </div>
    </div>
</template>

<script>
    export default {
        props: ['quote']
    }
</script>

<style scoped>
    div {
        border: 1px solid gray;
        box-shadow: 1px 1px 2px black;
        padding: 30px; 
        margin: 30px auto;
        text-align: center;
    }
    h1 {
        color: red;
    }
    
</style>
