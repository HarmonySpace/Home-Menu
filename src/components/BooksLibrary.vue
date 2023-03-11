<script setup>
import { ref } from 'vue'

let marks = ref([
    {
        title: "Pinterst",
        description: "For more inspiration",
        link: "https://www.pinterest.com/",
        color: "##e60024",
    },
    {
        title: "ChatGpt",
        description: "Do a chat with artificial intelligence. Contesta tus dudas y así",
        link: "https://www.pinterest.com/",
        color: "##e60024",
    },
    {
        title: "Pinterst",
        description: "For more inspiration",
        link: "https://www.pinterest.com/",
        color: "##e60024",
    },
    {
        title: "Pinterst",
        description: "For more inspiration",
        link: "https://www.pinterest.com/",
        color: "##e60024",
    },
    {
        title: "Pinterst",
        description: "For more inspiration",
        link: "https://www.pinterest.com/",
        color: "##e60024",
    },
    {
        title: "Pinterst",
        description: "For more inspiration",
        link: "https://www.pinterest.com/",
        color: "##e60024",
    },
])
</script>



<template>
    <div class="container">
        <div class="books">
            <div class="bookmark" v-for="mark in marks" :key="mark.title">
                <a :href="mark.link" class="bookmark-element">
                    <h1 class="bookmark-title">{{ mark.title }}</h1>
                    <p class="bookmark-description">{{ mark.description }}</p>
                </a>
            </div>
        </div>
    </div>
</template>



<style scoped>
.books {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    grid-gap: 0;
    justify-items: center;
    align-items: center;
    margin: 0;
    box-shadow: 15px 15px 25px #2c2c2c22;
}

.bookmark {
    display: flex;
    justify-content: start;
    align-content: end;
    height: 200px;
}

.bookmark-element {
    display: flex;
    justify-content: start;
    align-content: end;
    flex-wrap: wrap;
    text-align: start;
    text-decoration: none;
    padding: 15px;
    background-color: #1c1c1c;
}

.bookmark-title,
.bookmark-description {
    text-align: left;
    margin: 0;
}
</style>