<template>
  <div>
  <loading v-show="showLoading"/>
  <a-layout  v-if="!showLoading" :style="{height: '100%',width: '100%' }">
    <a-layout-sider collapsible :style="{height: '100%' }">
      <confNav/>
    </a-layout-sider>
    <a-layout :style="{width:'100%'}">
      <a-layout-content :style="{ background: '#fff',width:'100%' }"><confContent keep-alive/></a-layout-content>
      <!-- <a-layout-footer>Footer</a-layout-footer> -->
    </a-layout>
  </a-layout>
</div>
</template>

<script setup lang="ts">
import Loading from './Yolo/loading.vue'
import confNav from './Yolo/confNav.vue'
import confContent from './Yolo/confContent.vue'
import { ref } from 'vue'

defineProps<{ msg?: string }>()

const showLoading = ref(true);
setTimeout(() => {
  showLoading.value = false;
}, 3000)
</script>

<style>
div{
  height: 100%;
  width: 100%;
}
</style>