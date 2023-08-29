<template>
  <div>
    <div class="flex items-center justify-between">
      <div class="flex gap-3">
        <div
          class="w-6 h-6 rounded-full text-center text-md font-medium bg-amber-300 number"
        >
          {{ number }}
        </div>
        {{ title }}
      </div>
      <button v-on:click="isOpen = !isOpen">
        <img src="../../imgs/plus.svg" alt="plus" />
      </button>
    </div>

    <div :class="isOpen ? 'block' : 'hidden'">
      <slot> </slot>
    </div>
  </div>
</template>
<script>
export default {
  data: () => {
    return {
      isOpen: false,
    };
  },
  name: "Accordion",
  props: {
    title: String,
    number: Number,
  },
};
</script>
<style lang=""></style>
