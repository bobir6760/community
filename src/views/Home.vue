<template>
  <div class="home page">
    <Navbar />
    <Store />
    <Works />
    <Next />
    <Finish />
  </div>
</template>

<script>
import Navbar from "@/components/Navbar";
import Store from "@/components/Store";
import Works from "@/components/Works";
import Next from "@/components/Next";
import Finish from "@/components/Finish";
export default {
  name: "Home",
  components: { Navbar, Store, Works, Next, Finish },
};
</script>

<style lang="scss" scoped></style>
