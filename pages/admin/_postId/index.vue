<template>
    <div class="admin-post-page">
        <section class="update-form">
            <section class="update-form">
                <AdminPostForm :post="loadedPost" />
            </section>
        </section>
    </div>
</template>

<script>
import AdminPostForm from '@/components/Admin/AdminPostForm'
export default {
    layout: 'admin',
    components:{
        AdminPostForm
    },
    data() {
        return{
            loadedPost: {
                author: 'Perry',
                title: "shiiit",
                content: 'FUCK YEAH MAN',
                thumbnailLink: 'https://static.techspot.com/images2/news/bigimage/2018/07/2018-07-10-image-35.jpg'
            }
        }
    }
}
</script>

<style scoped>
    .update-form {
        width:90%;
        margin: 20px auto;
    }

    @media (min-width: 768px){
        .update-form {
            width:500px;
        }
    }
</style>

