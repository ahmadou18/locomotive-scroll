<template>
  <main id="scroll" class="h-screen w-full flex flex-row">
    <div
      class="h-screen w-screen bg-red-700 flex justify-center items-center text-7xl"
    >
      BLOC ONE
    </div>
    <div
      class="h-screen w-screen bg-blue-700 flex justify-center items-center text-7xl"
    >
      BLOC TWO
    </div>
    <div
      class="h-screen w-screen bg-green-700 flex justify-center items-center text-7xl"
    >
      BLOC THREE
    </div>
    <div
      class="h-screen w-screen bg-yellow-700 flex justify-center items-center text-7xl"
    >
      BLOC FOUR
    </div>
    <div
      class="h-screen w-screen bg-gray-700 flex justify-center items-center text-7xl"
    >
      BLOC FIVE
    </div>
  </main>
</template>

<script>
export default {
  name: "IndexPage",

  data() {
    return {
      lmS: null,
    };
  },

  mounted() {
    this.lmS = new this.locomotiveScroll({
      el: document.querySelector("#scroll"),
      smooth: true,
      direction: "horizontal",
    });
    console.log("lmS", this.lmS);
  },
};
</script>

<style lang="css">
#scroll {
  width: 1000%;
}
</style>
