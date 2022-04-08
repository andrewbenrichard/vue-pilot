<template>
  <div>
    <Script src="js/tilt.js" type="script" />
    <Link rel="stylesheet" href="https://unpkg.com/aos@next/dist/aos.css" />
    <Script src="https://unpkg.com/aos@next/dist/aos.js" />
    <div class="flex items-center justify-center w-full">
      <div
        class="text-center pt-[72px] w-[787px] flex flex-col justify-center items-center"
      >
        <h1 class="text-h1 font-medium text-dark-100 flex leading-[48px]">
          Pay Safe Anytime, Anywhere <img src="~assets/images/fight.svg" class="ml-1" />
        </h1>
        <h4 class="mt-8 leading-6 text-h4 text-dark-60">
          YODA is an the obligations of business it will frequently occur that pleasures
          have to be repudiated and annoyances accepted.
        </h4>
      </div>
    </div>
    <div class="w-full relative flex items-center justify-center mt-[99px]">
      <img
        data-tilt
        data-tilt-max="20"
        data-tilt-speed="400"
        data-tilt-perspective="10000"
        class="z-10 w-[calc(100%-356px)]"
        data-tilt-max-glare="2.8"
        data-tilt-glare
        data-aos="fade-up"
        data-aos-offset="200"
        data-aos-delay="100"
        data-aos-duration="2000"
        src="~assets/images/hero_1.png"
        alt=""
      />
      <div
        data-aos="fade-up"
        data-aos-offset="200"
        data-aos-delay="100"
        data-aos-duration="1600"
        class="circle absolute left-[1000px] top-[-70px]"
      >
        <img src="~assets/images/hero_assets/oval.svg" />
      </div>
      <div
        data-aos="fade-up"
        data-aos-offset="10"
        data-aos-delay="200"
        data-aos-duration="2000"
        class="left-[181px] bottom-0 absolute"
      >
        <img src="~assets/images/hero_assets/rectangle.svg" />
      </div>
      <div
        data-aos="fade-up"
        data-aos-offset="10"
        data-aos-delay="200"
        data-aos-duration="2000"
        class="left-[79.02px] w-[55px] top-[-48px] absolute"
      >
        <img src="~assets/images/hero_assets/high_five.png" />
      </div>
      <div class="left-[29.02px] bottom-[0px] absolute">
        <img src="~assets/images/hero_assets/boys_sily.svg" />
      </div>
      <div
        data-aos="fade-up"
        data-aos-offset="10"
        data-aos-delay="200"
        data-aos-duration="2000"
        class="left-[53.02px] top-[100px] absolute"
      >
        <img src="~assets/images/hero_assets/boys_bump.svg" />
      </div>
      <div
        data-aos="fade-up"
        data-aos-offset="10"
        data-aos-delay="200"
        data-aos-duration="2000"
        class="left-[10px] top-[203px] w-[50px] absolute"
      >
        <img src="~assets/images/hero_assets/cool.png" />
      </div>
      <div
        data-aos="fade-up"
        data-aos-offset="10"
        data-aos-delay="200"
        data-aos-duration="2000"
        class="right-[27px] top-[40px] w-7 absolute"
      >
        <img src="~assets/images/hero_assets/earth.png" />
      </div>
      <div
        data-aos="fade-up"
        data-aos-offset="10"
        data-aos-delay="200"
        data-aos-duration="2000"
        class="right-[50px] top-[144px] w-10 absolute"
      >
        <img src="~assets/images/hero_assets/angel.png" />
      </div>
      <div
        data-aos="fade-up"
        data-aos-offset="10"
        data-aos-delay="200"
        data-aos-duration="2000"
        class="right-[130px] top-[210px] w-12 absolute"
      >
        <img src="~assets/images/hero_assets/ebony_sily_face.svg" />
      </div>
      <div
        data-aos="fade-up"
        data-aos-offset="10"
        data-aos-delay="200"
        data-aos-duration="2000"
        class="right-[20px] top-[296px] absolute"
      >
        <img src="~assets/images/hero_assets/boys_glass.svg" />
      </div>
    </div>
    <div class="mt-[61px] w-full">
      <img class="mx-auto" src="~assets/images/hero_assets/clients.svg" />
    </div>
    <div class="mt-[140px] w-full flex flex-col justify-center items-center">
      <h1 class="text-h1 text-center font-medium text-dark-100 flex leading-[48px]">
        Built With Amazing Features
      </h1>
      <h4
        class="mt-[32px] leading-[30px] text-center text-base text-dark-80 font-normal max-w-[614px]"
      >
        These companies release their own versions of the operating systems with <br />
        minor changes, and yet always.
      </h4>
    </div>
    <div class="mt-[86px] mb-[139px]">
      <div class="flex justify-center w-full mt-[50px]">
        <div
          class="bg-primary-200 w-[142px] font-medium flex items-center cursor-pointer text-sm justify-center rounded-[7px] h-12 text-white"
        >
          <span class="text-white">Learn More</span>
        </div>
      </div>
    </div>
    <div class="w-full border border-solid border-dark-40"></div>
    <div class="mt-[158px]">
      <div class="grid grid-cols-2">
        <div class="pl-[160px] py-[87px]"></div>
        <div>
          <img src="~assets/images/section_assets/section_3.png" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>
<script>
import Button from "~/components/general/Button.vue"
export default {
  data() {
    return {
      hello: "Andrew",
    }
  },

  components: {
    Button,
  },
  mounted() {
    if (process.client) {
    }
  },
}
</script>

<style lang="scss" scoped>
.square {
  transform: rotate(-22deg) !important;
}
</style>
