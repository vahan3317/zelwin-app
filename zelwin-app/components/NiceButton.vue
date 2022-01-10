<template>
  <button
    class="bg-white border-2 border-black rounded-3xl min-w-[200px] min-h-[100px] flex p-4 text-white flex-col"
  >
    <div class="text-red-900"><slot name="header"> </slot></div>
    <div class="text-green-900"><slot name="body"> </slot></div>
    <slot> </slot>
  </button>
</template>

<script>
export default {}
</script>

<style></style>
