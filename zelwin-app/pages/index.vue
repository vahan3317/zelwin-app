<template>
<div class="container">
<NavBar />
  <Tutorial />
  </div>
</template>

<script>
import NavBar from "~/components/Nav-bar.vue";
export default {
    name: "IndexPage",
    components: { NavBar },
    otherName: "modal",
}
</script>
