<template>
  <div class="relative flex h-full">
    <div>
      <LayoutsSidebar2 :isCollapse="isCollapse" @openMenu="toggleMenu" />
    </div>
    <div
      class="px-0 lg:px-8 content-w pt-0 lg:pt-4 relative bg-[#F0F3F5]"
      :class="[
        { 'contentFull lg:left-[256px]': !isCollapse },
        { 'contentCollapse lg:left-[62px]': isCollapse },
      ]"
    >
      <LayoutsTopBar :isCollapse="isCollapse" @openMenu="toggleMenu" />

      <div class="px-4 mt-24 lg:px-0">
        <Nuxt />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      isCollapse: true,
      menu: [
        {
          header: "Main Navigation",
          hiddenOnCollapse: true,
        },
        {
          href: "/",
          title: "Dashboard",
          icon: "fa fa-user",
        },
        {
          href: "/charts",
          title: "Charts",
          icon: "fa fa-chart-area",
          child: [
            {
              href: "/charts/sublink",
              title: "Sub Link",
            },
          ],
        },
      ],
    }
  },
  computed: {
    mobChecker() {
      if (process.client && window.innerWidth < 768) {
        return window.innerWidth
      }
    },
  },
  watch: {
    mobChecker(val) {
      console.log(this.mobChecker)
    },
  },
  methods: {
    toggleMenu() {
      if (this.isCollapse) {
        this.isCollapse = false
        // console.log("here")
      } else {
        this.isCollapse = true
      }
    },
  },
}
</script>

<style lang="scss" scoped>
.content-w {
  width: calc(100% - 63px);
}
.content-w.contentFull {
  width: calc(100% - 256px);
  height: fit-content;
  // height: 100%;
}
.content-w.contentCollapse {
  width: calc(100% - 63px);
  height: fit-content;
  // height: 100%;
}
@media only screen and (max-width: 1024px) {
  .content-w.contentFull {
    width: 100%;
  }
  .content-w.contentCollapse {
    width: 100%;
  }
}
</style>
