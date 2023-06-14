<template>
    <div class="jumbotron">
        <img class="jumbotron-image" src="../../public/tokyo.jpg" alt="Tokyo Landscape">
        <h2>Visit Tokyo!</h2>
        <div class="likes">
            <button class="like-button" @click="likeIncrement()">👍</button>
            <div class="like-count">
                <h3>Likes: {{ likes }}</h3>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
                likes: 0
            }
        },
        methods: {
            likeIncrement() {
                this.likes++
            }
        }
    }
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

    div.jumbotron > div.likes {
        position: absolute;
        right: 1%;
        bottom: 1%;
        width: 10%;
    }

    div.jumbotron > div.likes > div.like-count,
    div.jumbotron > div.likes > button.like-button {
        background-color: rgba(0, 0, 0, 0.6);
        border-radius: 20px;
        margin: .5rem;
        padding: .3rem 1rem;
    }

    div.jumbotron > div.likes > button.like-button {
        font-size: 2rem;
    }
</style>