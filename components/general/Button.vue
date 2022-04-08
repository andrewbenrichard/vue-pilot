<template>
  <div
    :class="'bg-' + type"
    class="flex items-center cursor-pointer text-sm justify-center rounded-[7px] h-12 text-white"
  >
    <span class="text-[#ffffff]">{{ text }}</span>
  </div>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      default: null,
    },
    background: {
      type: String,
      default: null,
    },
    w: {
      type: String,
      default: null,
    },
  },
  computed: {
    type() {
      return this.background
    },
  },
}
</script>
