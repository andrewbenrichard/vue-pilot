<template>
  <div>
    <div v-if="error.statusCode === 404" class="text-center">
      <div class="relative flex justify-center w-full">
        <div class="w-[300px] h-[300px] rounded-full bg-white absolute top-0"></div>
        <img src="/assets/images/404.png" class="absolute top-24 w-[300px]" alt="" />
        <div class="relative top-[332px] text-center">
          <h1 class="text-[42px] font-light text-dark-100 mb3.5">404</h1>
          <p class="text-[42px] font-medium text-dark-100 mb3.5">Oops, Page not found!</p>
          <el-button to="/" type="primary"> Back to Home </el-button>
        </div>
      </div>
    </div>
    <div v-if="error.statusCode === 500" class="text-center">
      <div class="relative flex justify-center w-full">
        <div class="w-[300px] h-[300px] rounded-full bg-white absolute top-0"></div>
        <img src="/assets/images/500.png" class="absolute top-24 w-[300px]" alt="" />
        <div class="relative top-[332px] text-center">
          <h1 class="text-[42px] font-light text-dark-100 mb3.5">500</h1>
          <p class="text-[42px] font-medium text-dark-100 mb3.5">Something went wrong.</p>
          <el-button to="/" type="primary"> Back to Home </el-button>
        </div>
      </div>
    </div>
    <h1 v-else>An error occurred</h1>
  </div>
</template>

<script>
export default {
  props: ["error"],
  layout: "empty",
}
</script>

<style></style>
