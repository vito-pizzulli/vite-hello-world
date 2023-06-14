<template>
    <div class="jumbotron">
        <img class="jumbotron-image" src="../../public/tokyo.jpg" alt="Tokyo Landscape">
        <h2>Visit Tokyo!</h2>
    </div>
</template>

<script>
    
</script>

<style scoped>
    div.jumbotron {
        position: relative;
        border-radius: 20px;
    }
    div.jumbotron > img.jumbotron-image {
        width: 100%;
        border-radius: 20px;
    }

    div.jumbotron > h2 {
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        display: inline-block;
        font-size: 4rem;
        margin: 0;
        text-shadow: -1px -1px 0 #000, 1px -1px 0 #000, -1px 1px 0 #000, 1px 1px 0 #000;
        padding: 1rem;
        background-color: rgba(0, 0, 0, 0.5);
        border-radius: 20px;
    }
</style>