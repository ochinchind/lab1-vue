<template>
    <div class="blog-post" :style="{ backgroundImage: `url(${image})`, height: `${height}px` }">
        <div v-if="tags" class="tags">
            <div class="red">
                Science
            </div>
            <div class="green">
                Technology
            </div>
        </div>
        <div class="">
            <div class="blog-post-title">
                {{ title }}
            </div>
            <div class="blog-post-date">
                {{ date }}
            </div>
        </div>
        <div class="bottom-overlay"></div>
    </div>
    </template>
    
    <script>
    export default {
      name: 'HelloWorld',
      props: {
        image: String,
        title: String,
        date: String,
        height: Number,
        tags: Boolean
      }
    }
    </script>
    
    <!-- Add "scoped" attribute to limit CSS to this component only -->
    <style scoped>
    .blog-post {
        display: flex;
        flex-direction: column;
        justify-content: flex-end;
        width: 100%;
        background-size: cover;
        background-position: center;
        background-repeat: no-repeat;
        position: relative;
        overflow: hidden;
        height: 100%;
    }
    .blog-post-title {
        color: white;
        font-size: large;
        position: relative; 
        padding: 2rem 1rem;
        text-align: start;
    }
    .blog-post-date {
        padding: 0.5rem 1rem;
        color: rgb(215, 215, 215);
        font-size: medium;
        position: relative; 
        text-align: start;
    }
    .red {
        background-color: #ff0000;
        padding: 0.5rem 1rem;
        color: white;
        font-size: large;
    }
    .green {
        background-color: #007bff;
        padding: 0.5rem 1rem;
        color: white;
        font-size: large;
    }
    .tags {
        display: flex;
        gap: 10px;
        position: relative; 
        padding: 1rem;
    }

    .bottom-overlay {
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
        height: 10%;
        background: linear-gradient(to top, rgba(0, 0, 0, 0.7), rgba(0, 0, 0, 0));
    }
    </style>
    