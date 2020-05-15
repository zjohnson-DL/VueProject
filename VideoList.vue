        
        <!--trying to create a videolistitem for each
            element in the videos array. 
            then passing that video to videolistitem.
            videos is passed from app.vue as an array. 
        -->
<template>
    <ul>
        <VideoListItem 
        v-for="video in videos"
        v-bind:video="video"
        >
        </VideoListItem>

        <!--I tried the shorthand <VideoListItem v-for="video in videos" :video="video">  with the same result.
            
            Note that
            <VideoListItem :video="video"> works.
             -->

    </ul>
</template>

<script>
import VideoListItem from './VideoListItem.vue';

export default {
    name: 'VideoList',
    components:{
        VideoListItem
    },
    props: ['videos']
};
</script>

<style scoped>

</style>