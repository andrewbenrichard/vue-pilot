<template>
  <div
    :class="[{ 'w-full lg:w-[77%]': !isCollapse }, { 'w-full lg:w-[92%]': isCollapse }]"
    class="flex lg:mt-4 mt-0 py-3 pl-6 pr-[15px] bg-white fixed rounded-none lg:rounded-lg items-center z-20"
  >
    <div
      @click="sidebarToggle"
      class="flex justify-center w-8 h-8 rounded-full cursor-pointer bg-primary-400"
    >
      <svg
        width="24"
        height="24"
        viewBox="0 0 24 24"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M21.0004 6.6738C21.0004 8.7024 19.3552 10.3476 17.3266 10.3476C15.298 10.3476 13.6537 8.7024 13.6537 6.6738C13.6537 4.6452 15.298 3 17.3266 3C19.3552 3 21.0004 4.6452 21.0004 6.6738Z"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M10.3467 6.6738C10.3467 8.7024 8.7024 10.3476 6.6729 10.3476C4.6452 10.3476 3 8.7024 3 6.6738C3 4.6452 4.6452 3 6.6729 3C8.7024 3 10.3467 4.6452 10.3467 6.6738Z"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M21.0004 17.2622C21.0004 19.2908 19.3552 20.9351 17.3266 20.9351C15.298 20.9351 13.6537 19.2908 13.6537 17.2622C13.6537 15.2336 15.298 13.5884 17.3266 13.5884C19.3552 13.5884 21.0004 15.2336 21.0004 17.2622Z"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M10.3467 17.2622C10.3467 19.2908 8.7024 20.9351 6.6729 20.9351C4.6452 20.9351 3 19.2908 3 17.2622C3 15.2336 4.6452 13.5884 6.6729 13.5884C8.7024 13.5884 10.3467 15.2336 10.3467 17.2622Z"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
      </svg>
    </div>

    <div class="flex items-center ml-auto">
      <el-dropdown trigger="click" class="drop_notification" @command="handleMenu">
        <span class="el-dropdown-link">
          <div class="relative cursor-pointer">
            <svg
              width="24"
              height="24"
              viewBox="0 0 24 24"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <path
                fill-rule="evenodd"
                clip-rule="evenodd"
                d="M11.9961 2.51416C7.56185 2.51416 5.63519 6.5294 5.63519 9.18368C5.63519 11.1675 5.92281 10.5837 4.82471 13.0037C3.48376 16.4523 8.87614 17.8618 11.9961 17.8618C15.1152 17.8618 20.5076 16.4523 19.1676 13.0037C18.0695 10.5837 18.3571 11.1675 18.3571 9.18368C18.3571 6.5294 16.4295 2.51416 11.9961 2.51416Z"
                stroke="#B2BEC3"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M14.306 20.5122C13.0117 21.9579 10.9927 21.9751 9.68604 20.5122"
                stroke="#B2BEC3"
                stroke-width="1.5"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
            <svg
              class="absolute top-0 right-1"
              width="8"
              height="8"
              viewBox="0 0 8 8"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <rect width="8" height="8" rx="4" fill="#0010F7" />
            </svg>
          </div>
        </span>
        <el-dropdown-menu slot="dropdown" class="drop_notification">
          <el-dropdown-item command="setting">
            <span class="ml-2">Update your profile</span>
          </el-dropdown-item>
        </el-dropdown-menu>
      </el-dropdown>

      <div class="ml-6 cursor-pointer">
        <el-dropdown trigger="click" @command="handleMenu">
          <span class="el-dropdown-link">
            <img src="/assets/images/memoji-2.png" class="w-10 h-10" />
          </span>
          <el-dropdown-menu slot="dropdown">
            <el-dropdown-item command="setting">
              <div class="flex items-center">
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M12 9.5C13.3809 9.5 14.5 10.6191 14.5 12C14.5 13.3809 13.3809 14.5 12 14.5C10.6191 14.5 9.5 13.3809 9.5 12C9.5 10.6191 10.6191 9.5 12 9.5Z"
                    stroke="#130F26"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    fill-rule="evenodd"
                    clip-rule="evenodd"
                    d="M20.168 7.25025V7.25025C19.4845 6.05799 17.9712 5.65004 16.7885 6.33852C15.7598 6.93613 14.4741 6.18838 14.4741 4.99218C14.4741 3.61619 13.3659 2.5 11.9998 2.5V2.5C10.6337 2.5 9.52546 3.61619 9.52546 4.99218C9.52546 6.18838 8.23977 6.93613 7.21199 6.33852C6.02829 5.65004 4.51507 6.05799 3.83153 7.25025C3.14896 8.4425 3.55399 9.96665 4.73769 10.6541C5.76546 11.2527 5.76546 12.7473 4.73769 13.3459C3.55399 14.0343 3.14896 15.5585 3.83153 16.7498C4.51507 17.942 6.02829 18.35 7.21101 17.6625H7.21199C8.23977 17.0639 9.52546 17.8116 9.52546 19.0078V19.0078C9.52546 20.3838 10.6337 21.5 11.9998 21.5V21.5C13.3659 21.5 14.4741 20.3838 14.4741 19.0078V19.0078C14.4741 17.8116 15.7598 17.0639 16.7885 17.6625C17.9712 18.35 19.4845 17.942 20.168 16.7498C20.8515 15.5585 20.4455 14.0343 19.2628 13.3459H19.2618C18.2341 12.7473 18.2341 11.2527 19.2628 10.6541C20.4455 9.96665 20.8515 8.4425 20.168 7.25025Z"
                    stroke="#130F26"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>

                <span class="ml-2">Setting</span>
              </div></el-dropdown-item
            >
            <el-dropdown-item command="logout">
              <div class="flex items-center">
                <svg
                  width="24"
                  height="24"
                  viewBox="0 0 24 24"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M21.791 12.1206H9.75"
                    stroke="#130F26"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M18.8643 9.20459L21.7923 12.1206L18.8643 15.0366"
                    stroke="#130F26"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                  <path
                    d="M16.3597 7.63C16.0297 4.05 14.6897 2.75 9.35974 2.75C2.25874 2.75 2.25874 5.06 2.25874 12C2.25874 18.94 2.25874 21.25 9.35974 21.25C14.6897 21.25 16.0297 19.95 16.3597 16.37"
                    stroke="#130F26"
                    stroke-width="1.5"
                    stroke-linecap="round"
                    stroke-linejoin="round"
                  />
                </svg>
                <span class="ml-2">Log out</span>
              </div>
            </el-dropdown-item>
          </el-dropdown-menu>
        </el-dropdown>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    isCollapse: {
      type: Boolean,
    },
  },
  methods: {
    sidebarToggle() {
      if (this.isCollapse) {
        this.$emit("openMenu", true)
      } else {
        this.$emit("openMenu", false)
      }
    },
    handleMenu(command) {
      if (command == "setting") {
        this.$router.push("/profile/personal")
      } else {
        this.$router.push("/")
      }
    },
  },
}
</script>

<style lang="scss" scoped>
.el-dropdown-menu.el-popper.drop_notification {
  width: 300px;
}
</style>
