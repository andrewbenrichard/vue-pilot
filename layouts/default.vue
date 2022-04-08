<template>
  <div class="flex flex-col items-center w-full">
    <div class="max-w-[1440px]">
      <header class="h-16 w-full pl-[160px] pr-[161px] flex items-center">
        <img src="~assets/images/logo.svg" class="w-[158px]" />
        <div class="mx-auto flex text-sm text-dark-80 leading-[21px]">
          <a href="#" class="">Demos</a>
          <a href="#" class="px-[32px] text-primary">Features</a>
          <a href="#">Pricing</a>
        </div>
        <div class="flex items-center h-full">
          <a href="#" class="text-sm text-dark-80 mr-8 leading-[21px]">Sign Up</a>
          <div
            class="flex w-[102px] bg-primary items-center cursor-pointer text-sm justify-center rounded-[7px] h-12 text-white"
          >
            <span class="text-[#ffffff]">Login</span>
          </div>
        </div>
      </header>
      <Nuxt />
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped></style>
