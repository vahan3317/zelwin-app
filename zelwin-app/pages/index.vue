<template>
<div class="bg-[rgba(243,186,47,0.15)] w-full min-h-screen">
<NavBar />
  <!-- <Tutorial /> -->
  <WhiteCard/>
  
  </div>
</template>

<script>
import NavBar from "~/components/Nav-bar.vue";
import WhiteCard from "~/components/WhiteCard.vue";

export default {
    name: "IndexPage",
    components: { NavBar, WhiteCard},
    otherName: "modal",
}
</script>

