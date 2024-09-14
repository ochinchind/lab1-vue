<template>
    <div class="blog-post" :style="{ backgroundImage: `url(${image})`, height: `${height}px` }">
        <div class="">
            <div class="blog-post-title">
                {{ title }}
            </div>
            <div class="blog-post-date">
                {{ date }}
            </div>
        </div>
    </div>
    </template>
    
    <script>
    export default {
      name: 'HelloWorld',
      props: {
        image: String,
        title: String,
        date: String,
        height: Number
      }
    }
    </script>
    
    <!-- Add "scoped" attribute to limit CSS to this component only -->
    <style scoped>
    .blog-post {
        display: flex;
        width: 100%;
        background-size:cover;
        background-position: center; 
        background-repeat: no-repeat; 
        position: relative;
        overflow: hidden;
        align-items: end;
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
    </style>
    