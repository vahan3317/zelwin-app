<template>
  <button
    class="w-[295px]  border-2 border-[#DFEBF5]  rounded-[24px]   hover:bg-[#EFF3F8]      ">
    <div class="font-bold text-[28px] w-[212px] text-left pt-[16px] pl-[20px] md:text-[28px] md:w-[206px]  xl:text-[36px]   "><slot name="header"> </slot></div>
    <div class="text-[#DA554A] mt-[8px] text-[16px] font-semibold text-left pl-[20px] md:text-[16px] xl:text-[20px]    "><slot name="body1"> </slot></div>
    <div class="text-[14px] mt-[12px] mb-[12px]  text-[#828A97] text-left pb-[16px] pl-[20px]  md:text-[14px] xl:text-[20px]    "><slot name="body2"> </slot></div>
    <slot> </slot>
  </button>
</template>

<script>
export default {}
</script>

<style></style>
