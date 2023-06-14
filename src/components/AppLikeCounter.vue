<template>
    <div class="likes">
        <button class="like-button" @click="likeIncrement()">👍</button>
        <div class="like-count">
            <h3>Likes: {{ likes }}</h3>
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
    div.likes {
        position: absolute;
        right: 1%;
        bottom: 1%;
        width: 10%;
    }

    div.likes > div.like-count,
    div.likes > button.like-button {
        background-color: rgba(0, 0, 0, 0.6);
        border-radius: 20px;
        margin: .5rem;
        padding: .3rem 1rem;
    }

    div.likes > button.like-button {
        font-size: 2rem;
    }
</style>