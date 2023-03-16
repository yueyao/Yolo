<template>
  <div class="loading">Yolo</div>
</template>

<script lang="ts">
export default {

}
</script>

<style>
.loading {
  width: 50px;
  height: 50px;
  position: absolute;
  top:50%;
  left: calc(50% - 25px);
  border: 3px solid #000;
  border-top-color: transparent;
  border-radius: 100%;
  animation: circle infinite 0.75s linear;
  color:hsl(219, 75%, 47%);
}

@keyframes circle {
  0% {
    transform: rotate(0);
  }
  100% {
    transform: rotate(360deg);
  }
}

</style>