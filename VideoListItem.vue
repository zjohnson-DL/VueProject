<template>
    <li>
        {{video.snippet.title}}
        </li>
</template>

<script>
export default {
    name: 'VideoListItem',
    
    //video being passed from videolistvue
    props: ['video']
}
</script>