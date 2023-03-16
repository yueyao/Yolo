<template>
  <div :style="{width:'100%'}">
    <!-- <div id="chatgpt"></div> -->
    <iframe src="https://chat.jungo.fi/"></iframe>
  </div>
</template>

<script setup lang="ts">
// @ts-ignore;
import ciframe from 'iframe';


// const frame = ciframe({ container: document.querySelector('#chatgpt') , src: "https://chat.jungo.fi/" })
// setTimeout(() => {
//     frame.resize()
// },1000)


</script>

<style>
div{
    height:100%;
    overflow: hidden;
}
iframe{
    border: none;
    width:100%;
    height:100%;
}
</style>