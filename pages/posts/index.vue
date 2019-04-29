<template>
    <div class="c-page__posts">
        <PostList />
    </div>
</template>

<script>
import PostList from '@/components/posts/PostList'
export default {
    components:{
        PostList
    }
}
</script>



<style scoped>
.c-page__posts{
    display:flex;
    justify-content: center;
    align-items: center;
}


</style>
