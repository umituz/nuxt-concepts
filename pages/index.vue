<template>
    <div>
        <PostList :posts="fetchedPosts" />
        <About />
    </div>
</template>
<script>
    import PostList from '~/components/post/PostList';
    import About from '~/components/home/About';
    export default {
        components : {
            PostList,
            About
        },
        data(){
            return {
                fetchedPosts:[]
            }
        },
        created(){},
        asyncData(context,callback){
            setTimeout(() => {
                callback(null,{
                    fetchedPosts : [
                        {
                            id:1,
                            title:'1.yazı Vuejs Öğrenimi',
                            subTitle:'1.yazı Vuejs javascript kütüphanesi view katmanına odaklanır.',
                            text:'1.yazı Vuejs Evan You tarafından yazılan bir javascript kütüphanesidir. Gelişiminde Laravel php frameworkünün büyük katkıları vardır.',
                            author:'1.yazı Ümit UZ'
                        },
                        {
                            id:2,
                            title:'2.yazı Vuejs Öğrenimi',
                            subTitle:'2.yazı Vuejs javascript kütüphanesi view katmanına odaklanır.',
                            text:'2.yazı Vuejs Evan You tarafından yazılan bir javascript kütüphanesidir. Gelişiminde Laravel php frameworkünün büyük katkıları vardır.',
                            author:'2.yazı Ümit UZ'
                        },
                        {
                            id:3,
                            title:'3.yazı Vuejs Öğrenimi',
                            subTitle:'3.yazı Vuejs javascript kütüphanesi view katmanına odaklanır.',
                            text:'3.yazı Vuejs Evan You tarafından yazılan bir javascript kütüphanesidir. Gelişiminde Laravel php frameworkünün büyük katkıları vardır.',
                            author:'3.yazı Ümit UZ'
                        },
                        {
                            id:4,
                            title:'4.yazı Vuejs Öğrenimi',
                            subTitle:'4.yazı Vuejs javascript kütüphanesi view katmanına odaklanır.',
                            text:'4.yazı Vuejs Evan You tarafından yazılan bir javascript kütüphanesidir. Gelişiminde Laravel php frameworkünün büyük katkıları vardır.',
                            author:'4.yazı Ümit UZ'
                        },
                        {
                            id:5,
                            title:'5.yazı Vuejs Öğrenimi',
                            subTitle:'5.yazı Vuejs javascript kütüphanesi view katmanına odaklanır.',
                            text:'5.yazı Vuejs Evan You tarafından yazılan bir javascript kütüphanesidir. Gelişiminde Laravel php frameworkünün büyük katkıları vardır.',
                            author:'5.yazı Ümit UZ'
                        },
                        {
                            id:6,
                            title:'6.yazı Vuejs Öğrenimi',
                            subTitle:'6.yazı Vuejs javascript kütüphanesi view katmanına odaklanır.',
                            text:'6.yazı Vuejs Evan You tarafından yazılan bir javascript kütüphanesidir. Gelişiminde Laravel php frameworkünün büyük katkıları vardır.',
                            author:'6.yazı Ümit UZ'
                        },
                    ]
                });
            },1000);
        }
    }
</script>
<style scoped></style>