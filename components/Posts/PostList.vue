<template>
    <section class="post-list">
        <PostPreview 
            id="1" 
            :is-admin="isAdmin"
            thumbnail="https://assets.thehansindia.com/h-upload/2021/07/31/1600x960_1092805-tech.jpg"
            title="Hello!" 
            previewText="This is my First Post!" />
        <PostPreview 
            id="2" 
            :is-admin="isAdmin"
            thumbnail="https://assets.thehansindia.com/h-upload/2021/07/31/1600x960_1092805-tech.jpg"
            title="Hello!" 
            previewText="This is my Second Post!" />
        <PostPreview 
            id="3" 
            :is-admin="isAdmin"
            thumbnail="https://assets.thehansindia.com/h-upload/2021/07/31/1600x960_1092805-tech.jpg"
            title="Hello!" 
            previewText="This is my Third Post!" />
    </section>
</template>

<script>
import PostPreview from '~/components/Posts/PostPreview.vue'

export default {
    components: {
        PostPreview
    },
    props: {
        isAdmin: {
            type: Boolean,
            default: false
        }
    }
}
</script>

<style>
    .post-list {
        display: flex;
        padding: 20px;
        box-sizing: border-box;
        flex-wrap: wrap;
        align-items: center;
        justify-content: center;
    }
</style>