<template>
  <div class="w-[736px] bg-white h-[424px] rounded-2xl p-5 flex">
    <div class="relative mr-5">
      <div
        class="absolute top-2.5 right-2.5 w-8 h-8 p-2 rounded-full cursor-pointer bg-dark-10"
      >
        <img src="/assets/images/heart-fill.svg" alt="" />
      </div>
      <img src="/assets/images/card-img.png" alt="" />
    </div>
    <div>
      <div class="flex">
        <img src="/assets/images/User-Icon.png" alt="" />
        <div class="ml-2.5">
          <p class="m-0 text-[#B7B7B7] text-xs">Owned by</p>
          <p class="m-0 text-sm font-medium text-dark-100">Daniel Malbrook</p>
        </div>
      </div>
      <p class="m-0 mt-6 text-2xl font-semibold text-dark-100">
        Contemporary Colour Abstract Painting
      </p>
      <div
        class="flex mt-4 py-3 pr-5 bg-[#F9F9F9] rounded-xl before:absolute before:bg-primary before:w-[5px] before:h-[56px] before:rounded-lg items-center"
      >
        <p class="ml-4 text-sm font-medium text-[#4F4F4F]">
          Current <br />
          Bid
        </p>
        <div class="ml-auto">
          <div class="flex">
            <img src="/assets/images/eth.svg" alt="" />
            <div>
              <p class="m-0 text-xl font-medium text-primary">0.00050 ETH</p>
              <p class="m-0 text-[#C3C9CE] font-medium text-[10px]">$1,732.23</p>
            </div>
          </div>
        </div>
      </div>
      <div
        class="flex mt-4 py-3 pr-5 bg-[#F9F9F9] rounded-xl before:absolute before:bg-primary before:w-[5px] before:h-[56px] before:rounded-lg items-center"
      >
        <p class="ml-4 text-sm font-medium text-[#4F4F4F]">
          Auction
          <br />
          Ending In
        </p>
        <div class="ml-auto">
          <div class="flex">
            <div>
              <p class="m-0 text-xl font-medium text-primary">{{ countdown.hours }}</p>
              <p class="m-0 text-[#C3C9CE] font-medium text-[10px]">Hours</p>
            </div>
            <div class="mx-3 text-xl">:</div>
            <div>
              <p class="m-0 text-xl font-medium text-primary">{{ countdown.minutes }}</p>
              <p class="m-0 text-[#C3C9CE] font-medium text-[10px]">Mins</p>
            </div>
            <div class="mx-3 text-xl">:</div>
            <div>
              <p class="m-0 text-xl font-medium text-primary">{{ countdown.seconds }}</p>
              <p class="m-0 text-[#C3C9CE] font-medium text-[10px]">Secs</p>
            </div>
          </div>
        </div>
      </div>
      <div class="flex w-full mt-3 5">
        <button
          class="w-[174px] h-10 rounded-full text-sm font-medium text-white bg-primary"
        >
          Place Bid
        </button>
        <button
          class="w-[174px] h-10 rounded-full text-sm font-medium bg-white border-solid text-primary border-primary border-[1px] ml-[18px]"
        >
          View Art
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  layout: "authPages",
  data() {
    return {
      countdown: {
        hours: "00",
        minutes: "00",
        seconds: "00",
      },
    }
  },
  created() {
    this.auctionTimer()
  },
  methods: {
    auctionTimer() {
      let self = this
      // Set the date we're counting down to
      var countDownDate = new Date("Jan 5, 2024 15:37:25").getTime()

      // Update the count down every 1 second
      var x = setInterval(function () {
        // Get today's date and time
        var now = new Date().getTime()

        // Find the distance between now and the count down date
        var distance = countDownDate - now

        // Time calculations for days, hours, minutes and seconds
        var days = Math.floor(distance / (1000 * 60 * 60 * 24))
        var hours = Math.floor((distance % (1000 * 60 * 60 * 24)) / (1000 * 60 * 60))
        var minutes = Math.floor((distance % (1000 * 60 * 60)) / (1000 * 60))
        var seconds = Math.floor((distance % (1000 * 60)) / 1000)

        // Display the result in the element with id="demo"
        self.countdown.hours = hours
        self.countdown.minutes = minutes
        self.countdown.seconds = seconds
        // console.log(days + "d " + hours + "h " + minutes + "m " + seconds + "s ")

        // If the count down is finished, write some text
        if (distance < 0) {
          clearInterval(x)
          console.log("EXPIRED")
        }
      }, 1000)
    },
  },
}
</script>

<style></style>
