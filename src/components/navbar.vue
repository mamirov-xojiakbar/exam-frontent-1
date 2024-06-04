<template>
  <div class="bg-tint_blue/80 w-full fixed z-20">
    <div class="md:container flex justify-between items-center px-5 py-5 md:px-0 md:py-0">
      <img src="../../public/Logo.png" alt="" />


      <button class="flex items-center md:hidden">
        <svg
          xmlns="http://www.w3.org/2000/svg"
          width="3em"
          height="3em"
          viewBox="0 0 256 256"
        >
          <path
            fill="white"
            d="M228 128a12 12 0 0 1-12 12H40a12 12 0 0 1 0-24h176a12 12 0 0 1 12 12M40 76h176a12 12 0 0 0 0-24H40a12 12 0 0 0 0 24m176 104H40a12 12 0 0 0 0 24h176a12 12 0 0 0 0-24"
          />
        </svg>
      </button>

      <div
        class="md:flex gap-[40px] items-center font-medium text-[16px] leading-[28px] hidden"
      >
        <router-link
          to="/"
          class="[&.router-link-active]:text-white text-navbar_text"
          >Home</router-link
        >
        <router-link
          to="/about"
          class="[&.router-link-active]:text-white text-navbar_text"
          >About us</router-link
        >
        <router-link
          to="/pricing"
          class="[&.router-link-active]:text-white text-navbar_text"
          >Pricing</router-link
        >
        <router-link
          to="/work"
          class="[&.router-link-active]:text-white text-navbar_text"
          >Work</router-link
        >
        <router-link
          to="/blog"
          class="[&.router-link-active]:text-white text-navbar_text"
          >Blog</router-link
        >
        <button
          class="border-[2px] border-navbar_button py-[16px] px-[48px] rounded-[41px] my-[16px] text-white"
        >
          Contact us
        </button>
      </div>
    </div>
    
  </div>
</template>

<script setup>
</script>

<style lang="scss" scoped></style>
