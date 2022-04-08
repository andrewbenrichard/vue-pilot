<template>
  <div class="w-[256px] h-full bg-white py-6 flex flex-col fixed">
    <img src="/assets/images/Logo.png" class="w-[158px] px-6 mb-[38px]" />
    <nuxt-link
      to="/dashboard"
      class="flex items-center w-full h-12 px-6 py-3 cursor-pointer"
    >
      <svg
        width="24"
        height="24"
        viewBox="0 0 24 24"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M9.07861 16.1354H14.8936"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M2.3999 13.713C2.3999 8.082 3.0139 8.475 6.3189 5.41C7.7649 4.246 10.0149 2 11.9579 2C13.8999 2 16.1949 4.235 17.6539 5.41C20.9589 8.475 21.5719 8.082 21.5719 13.713C21.5719 22 19.6129 22 11.9859 22C4.3589 22 2.3999 22 2.3999 13.713Z"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
      </svg>

      <span class="ml-2 text-sm text-dark-80">Dashboard</span>
    </nuxt-link>
    <nuxt-link
      to="/appointments"
      class="flex items-center w-full h-12 px-6 py-3 cursor-pointer"
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
          d="M2.74976 12.776C2.74976 5.81995 5.06876 3.50195 12.0238 3.50195C18.9798 3.50195 21.2988 5.81995 21.2988 12.776C21.2988 19.732 18.9798 22.05 12.0238 22.05C5.06876 22.05 2.74976 19.732 2.74976 12.776Z"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M3.02515 9.32422H21.0331"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M16.4284 13.2612H16.4374"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M12.0289 13.2612H12.0379"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M7.62148 13.2612H7.63048"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M16.4284 17.1133H16.4374"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M12.0289 17.1133H12.0379"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M7.62148 17.1133H7.63048"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M16.033 2.05029V5.31229"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M8.02466 2.05029V5.31229"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
      </svg>
      <span class="ml-2 text-sm text-dark-80">Appointments</span>
    </nuxt-link>
    <nuxt-link
      to="/projects"
      class="flex items-center w-full h-12 px-6 py-3 cursor-pointer"
    >
      <svg
        width="24"
        height="24"
        viewBox="0 0 24 24"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M11.9612 16.5167V13.8887"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M21.0895 11.4775L21.0605 11.4985C18.6385 12.9905 15.4405 13.8915 11.9565 13.8915C8.47252 13.8915 5.28352 12.9905 2.86252 11.4985L2.83252 11.4775"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M2.75024 13.3505C2.75024 7.19846 5.05324 5.14746 11.9612 5.14746C18.8702 5.14746 21.1722 7.19846 21.1722 13.3505C21.1722 19.5025 18.8702 21.5535 11.9612 21.5535C5.05324 21.5535 2.75024 19.5025 2.75024 13.3505Z"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M15.2237 5.3692V4.7392C15.2237 3.4752 14.3007 2.4502 13.1637 2.4502H10.7587C9.62173 2.4502 8.69873 3.4752 8.69873 4.7392V5.3692"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
      </svg>

      <span class="ml-2 text-sm text-dark-80">Projects</span>
    </nuxt-link>
    <nuxt-link
      to="/clients"
      class="flex items-center w-full h-12 px-6 py-3 cursor-pointer"
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
          d="M11.9726 20.3681C8.73355 20.3681 5.96655 19.8781 5.96655 17.9161C5.96655 15.9541 8.71555 14.2461 11.9726 14.2461C15.2116 14.2461 17.9786 15.9381 17.9786 17.8991C17.9786 19.8601 15.2296 20.3681 11.9726 20.3681Z"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M11.9726 11.4485C14.0986 11.4485 15.8226 9.72551 15.8226 7.59951C15.8226 5.47351 14.0986 3.74951 11.9726 3.74951C9.84657 3.74951 8.12257 5.47351 8.12257 7.59951C8.11657 9.71751 9.82657 11.4415 11.9456 11.4485H11.9726Z"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M18.362 10.3915C19.599 10.0605 20.511 8.93254 20.511 7.58954C20.511 6.18854 19.518 5.01854 18.196 4.74854"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M18.9431 13.5442C20.6971 13.5442 22.1951 14.7332 22.1951 15.7952C22.1951 16.4202 21.6781 17.1012 20.8941 17.2852"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M5.58384 10.3915C4.34584 10.0605 3.43384 8.93254 3.43384 7.58954C3.43384 6.18854 4.42784 5.01854 5.74884 4.74854"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M5.00176 13.5442C3.24776 13.5442 1.74976 14.7332 1.74976 15.7952C1.74976 16.4202 2.26676 17.1012 3.05176 17.2852"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
      </svg>

      <span class="ml-2 text-sm text-dark-80">Clients</span>
    </nuxt-link>
    <nuxt-link to="/store" class="flex items-center w-full h-12 px-6 py-3 cursor-pointer">
      <svg
        width="24"
        height="24"
        viewBox="0 0 24 24"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M5.52377 7C9.41427 5.74386 13.9724 5.45573 16 5.5C18.0276 5.54427 18.8831 6.2663 19.5 7.5C20.5 9.5 20.289 14.4881 18.5 16.0871C16.712 17.6861 9.33015 17.8381 6.87015 16.0871C4.27115 14.2361 5.629 9.192 5.544 5.743C5.595 3.813 3.5 3.5 3.5 3.5"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          d="M13 10.5H15.773"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M7.26399 20.1274C7.56399 20.1274 7.80799 20.3714 7.80799 20.6714C7.80799 20.9724 7.56399 21.2164 7.26399 21.2164C6.96299 21.2164 6.71899 20.9724 6.71899 20.6714C6.71899 20.3714 6.96299 20.1274 7.26399 20.1274Z"
          fill="#130F26"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
        <path
          fill-rule="evenodd"
          clip-rule="evenodd"
          d="M17.5955 20.1274C17.8965 20.1274 18.1405 20.3714 18.1405 20.6714C18.1405 20.9724 17.8965 21.2164 17.5955 21.2164C17.2955 21.2164 17.0515 20.9724 17.0515 20.6714C17.0515 20.3714 17.2955 20.1274 17.5955 20.1274Z"
          fill="#130F26"
          stroke="#130F26"
          stroke-width="1.5"
          stroke-linecap="round"
          stroke-linejoin="round"
        />
      </svg>

      <span class="ml-2 text-sm text-dark-80">Store</span>
    </nuxt-link>
    <hr class="mx-6 mt-auto" />
    <div class="mt-[30px] flex items-center px-6">
      <img src="/assets/images/memoji-2.png" class="w-8 h-8 mr-2 cursor-pointer" />
      <div class="">
        <p class="m-0 text-sm text-dark-100">Jane Doe</p>
        <p class="m-0 text-xs font-semibold cursor-pointer text-dark-80">View Profile</p>
      </div>
      <svg
        class="ml-auto cursor-pointer"
        width="24"
        height="24"
        viewBox="0 0 24 24"
        fill="none"
        xmlns="http://www.w3.org/2000/svg"
      >
        <path
          d="M3.34006 17.0001C2.91733 16.2691 2.58873 15.4875 2.36206 14.6741C2.85537 14.4232 3.26965 14.0407 3.55909 13.569C3.84852 13.0972 4.00183 12.5546 4.00203 12.0012C4.00224 11.4477 3.84934 10.905 3.56026 10.4331C3.27118 9.96112 2.85718 9.57834 2.36406 9.32707C2.8161 7.69255 3.67679 6.20002 4.86506 4.99007C5.32915 5.29179 5.86768 5.45923 6.42104 5.47385C6.9744 5.48847 7.52101 5.3497 8.00039 5.0729C8.47977 4.7961 8.87321 4.39207 9.13719 3.90551C9.40116 3.41895 9.52537 2.86884 9.49606 2.31607C11.1382 1.89169 12.8613 1.89238 14.5031 2.31807C14.474 2.87083 14.5985 3.42086 14.8626 3.90728C15.1268 4.39369 15.5204 4.79754 15.9999 5.07413C16.4794 5.35071 17.026 5.48925 17.5793 5.47442C18.1327 5.45958 18.6711 5.29195 19.1351 4.99007C19.7141 5.58007 20.2281 6.25107 20.6601 7.00007C21.0931 7.74907 21.4171 8.53007 21.6381 9.32607C21.1448 9.57697 20.7305 9.95944 20.441 10.4312C20.1516 10.9029 19.9983 11.4455 19.9981 11.999C19.9979 12.5524 20.1508 13.0951 20.4399 13.5671C20.7289 14.039 21.1429 14.4218 21.6361 14.6731C21.184 16.3076 20.3233 17.8001 19.1351 19.0101C18.671 18.7083 18.1324 18.5409 17.5791 18.5263C17.0257 18.5117 16.4791 18.6504 15.9997 18.9272C15.5204 19.204 15.1269 19.6081 14.8629 20.0946C14.599 20.5812 14.4748 21.1313 14.5041 21.6841C12.862 22.1084 11.1388 22.1078 9.49706 21.6821C9.52611 21.1293 9.40166 20.5793 9.13748 20.0929C8.8733 19.6064 8.4797 19.2026 8.00023 18.926C7.52076 18.6494 6.97412 18.5109 6.42079 18.5257C5.86746 18.5406 5.32902 18.7082 4.86506 19.0101C4.27405 18.407 3.76166 17.7317 3.34006 17.0001ZM9.00006 17.1961C10.0657 17.8107 10.8669 18.7971 11.2501 19.9661C11.7491 20.0131 12.2501 20.0141 12.7491 19.9671C13.1325 18.7979 13.9341 17.8115 15.0001 17.1971C16.0653 16.5808 17.3206 16.3795 18.5251 16.6321C18.8151 16.2241 19.0651 15.7891 19.2731 15.3341C18.4525 14.4175 17.9992 13.2303 18.0001 12.0001C18.0001 10.7401 18.4701 9.56307 19.2731 8.66607C19.0636 8.21122 18.8125 7.7767 18.5231 7.36807C17.3193 7.62038 16.0649 7.41954 15.0001 6.80407C13.9344 6.18944 13.1332 5.20305 12.7501 4.03407C12.2511 3.98707 11.7501 3.98607 11.2511 4.03307C10.8677 5.20221 10.0661 6.18863 9.00006 6.80307C7.93484 7.41938 6.67954 7.62059 5.47506 7.36807C5.18563 7.77635 4.93519 8.21093 4.72706 8.66607C5.54763 9.58263 6.00094 10.7699 6.00006 12.0001C6.00006 13.2601 5.53006 14.4371 4.72706 15.3341C4.93653 15.7889 5.1876 16.2234 5.47706 16.6321C6.68078 16.3798 7.93527 16.5806 9.00006 17.1961ZM12.0001 15.0001C11.2044 15.0001 10.4413 14.684 9.87874 14.1214C9.31613 13.5588 9.00006 12.7957 9.00006 12.0001C9.00006 11.2044 9.31613 10.4414 9.87874 9.87875C10.4413 9.31614 11.2044 9.00007 12.0001 9.00007C12.7957 9.00007 13.5588 9.31614 14.1214 9.87875C14.684 10.4414 15.0001 11.2044 15.0001 12.0001C15.0001 12.7957 14.684 13.5588 14.1214 14.1214C13.5588 14.684 12.7957 15.0001 12.0001 15.0001ZM12.0001 13.0001C12.2653 13.0001 12.5196 12.8947 12.7072 12.7072C12.8947 12.5196 13.0001 12.2653 13.0001 12.0001C13.0001 11.7348 12.8947 11.4805 12.7072 11.293C12.5196 11.1054 12.2653 11.0001 12.0001 11.0001C11.7348 11.0001 11.4805 11.1054 11.293 11.293C11.1054 11.4805 11.0001 11.7348 11.0001 12.0001C11.0001 12.2653 11.1054 12.5196 11.293 12.7072C11.4805 12.8947 11.7348 13.0001 12.0001 13.0001Z"
          fill="#2D3436"
        />
      </svg>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style></style>
