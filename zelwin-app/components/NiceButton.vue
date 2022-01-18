<template>
  <button
    class="flex flex-col w-[295px]  md:min-w-[206px]  lg:w-[278px] xl:w-[331px] border-2 border-[#DFEBF5]  rounded-[24px]   hover:bg-[#EFF3F8] xl:w-[331px]  pt-[16px]  px-[20px] pb-[16px] lg:pt-[20px] lg:px-[24px] xl:pt-[24] xl:px-[24px]  ">
    <div class="font-bold text-[28px] md:text-[28px]       "><slot name="header"> </slot></div>
    <div class="text-[#DA554A]   text-[16px] font-semibold md:text-[16px] xl:text-[20px] mt-[8px]      "><slot name="body1"> </slot></div>
    <div class="text-[14px]   text-[#828A97]    md:text-[14px] xl:text-[20px]   mt-[10px]  "><slot name="body2"> </slot></div>
    <slot> </slot>
  </button>
</template>

<script>
export default {}
</script>

<style></style>
