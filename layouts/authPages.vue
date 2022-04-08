<template>
  <div class="flex justify-center w-full h-full pt-7 md:pt-24 bg-primary auth_bg">
    <Nuxt />
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.auth_bg {
  background-image: url("/assets/images/bg_pattern.svg");
  background-position: bottom;
  background-repeat: no-repeat;
  background-size: cover;
}
</style>
