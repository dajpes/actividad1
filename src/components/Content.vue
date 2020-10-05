<template>
  <div>
    <Slider  class="mt-10 "/>
    <Info />
    <Contact />
  </div>
</template>

<script>
import Slider from "./Slider";
import Info from "./Info";
import Contact from "./Contact";
export default {
  components: {
    Slider,
    Info,
    Contact,
  },
};
</script>

<style lang="scss" scoped></style>
