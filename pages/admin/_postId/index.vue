<template>
    <div>
        <PostForm :is-update="true"/>
    </div>
</template>
<script>
    import PostForm from '~/components/admin/PostForm'
    export default {
        components:{
            PostForm
        }
    }
</script>