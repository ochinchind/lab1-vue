<template>
<div class="bg-body-gray blog-content">
    <div class="container">
        <div class="blog-content-posts">
            <div class="blog-content-posts-post-area">
                <BlogContentPost image="'https://physicsworld.com/wp-content/uploads/2018/03/rexfeatures_2048826b-web.jpg'" title="The AI removes objects magically moving from video" date="July 19, 2019" height="300"/>
                <BlogContentPost image="'https://physicsworld.com/wp-content/uploads/2018/03/rexfeatures_2048826b-web.jpg'" title="The AI removes objects magically moving from video" date="July 19, 2019" height="300" />
            </div>
            <div class="blog-content-posts-post-area">
                <BlogContentPost image="'https://physicsworld.com/wp-content/uploads/2018/03/rexfeatures_2048826b-web.jpg'" title="The AI removes objects magically moving from video" date="July 19, 2019" tags="true" />
            </div>
            <div class="blog-content-posts-post-area">
                <BlogContentPost image="'https://physicsworld.com/wp-content/uploads/2018/03/rexfeatures_2048826b-web.jpg'" title="The AI removes objects magically moving from video" date="July 19, 2019" height="300"/>
                <BlogContentPost image="'https://physicsworld.com/wp-content/uploads/2018/03/rexfeatures_2048826b-web.jpg'" title="The AI removes objects magically moving from video" date="July 19, 2019" height="300"/>
            </div>
        </div>
    </div>
</div>
</template>

<script>
import BlogContentPost from './BlogContentPost.vue';

export default {
name: 'HelloWorld',
components: {
BlogContentPost  // Register the BlogContentPost component here
},
props: {
    msg: String
}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.bg-body-gray {
    background-color: rgba(248, 249, 250, 1);
}
.blog-content {
    padding-top: 3rem;
    padding-bottom: 3rem;
}
.container {
    max-width: 1320px;
    width:100%;
    margin-right: auto;
    margin-left: auto;
}
.blog-content-posts {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between; 
}
.blog-content-posts-post-area {
    flex: 1 1 30%; 
    margin-bottom: 1rem;
    margin-right: 1rem;
    box-sizing: border-box;
    display: grid;
    gap: 2rem; 
}
.blog-content-posts-post-area:nth-child(3n) {
    margin-right: 0;
}
</style>
