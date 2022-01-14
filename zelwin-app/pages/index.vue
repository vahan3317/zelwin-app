<template>
<div class=" ">
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

