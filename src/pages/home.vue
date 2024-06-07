<template>
  <!-- start header -->
  <header class="bg-tint_blue pt-[110px] md:pt-[200px] md:pb-[128px] pb-[70px]">
    <div class="container md:flex md:gap-[60px] px-5 md:px-0">
      <div class="text-white md:pr-[40px]">
        <h1 class="font-semibold md:text-[54px] text-[30px] md:leading-[74px] text-center md:text-start">
          Building stellar websites for early startups
        </h1>
        <p class="font-medium text-[16px] leading-[28px] mt-[24px] text-center md:text-start">
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do
          eiusmod tempor incididunt.
        </p>

        <div class="md:flex mt-[48px] items-center gap-[40px] hidden">
          <router-link to="/work"
            class="bg-header_button font-semibold text-[18px] leading-[32px] px-[56px] py-[16px] rounded-[41px] text-black"
          >
            View our work
          </router-link>
          <router-link to="/pricing" class="flex items-center gap-[14px]"
            >View Pricing <img src="../../public/Arrow.png" alt=""
          /></router-link>
        </div>
      </div>

      <div class="md:flex md:w-full pt-10 md:justify-end">
        <img src="../../public/Illustration.svg" alt="" class="w-full "/>

        <div class="flex mt-[48px] items-center gap-[40px] md:hidden">
          <router-link to="/work"
            class="bg-header_button font-semibold text-[18px] leading-[32px] px-[30px] md:px-[56px] py-[16px] rounded-[41px] text-black"
          >
            View our work
          </router-link>
          <router-link to="/pricing" class="flex items-center gap-[14px] text-white"
            >View Pricing <img src="../../public/Arrow.png" alt=""
          /></router-link>
        </div>
      </div>
    </div>
  </header>
  <!-- end header -->

  <!-- start our project -->
  <section class="mt-[57px] md:container px-5 md:px-0">
    <div class="md:my-10">
      <div class="flex justify-between items-center">
        <h2 class="text-our_project text-[17px] md:text-[48px] font-semibold">
          View our projects
        </h2>
        <router-link to="/pricing" class="flex items-center text-our_project">
          <span class="mr-2">View pricing</span>
          <svg
            width="25"
            height="12"
            viewBox="0 0 25 12"
            fill="none"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              d="M24.5303 6.53033C24.8232 6.23744 24.8232 5.76256 24.5303 5.46967L19.7574 0.696699C19.4645 0.403806 18.9896 0.403806 18.6967 0.696699C18.4038 0.989593 18.4038 1.46447 18.6967 1.75736L22.9393 6L18.6967 10.2426C18.4038 10.5355 18.4038 11.0104 18.6967 11.3033C18.9896 11.5962 19.4645 11.5962 19.7574 11.3033L24.5303 6.53033ZM0 6.75H24V5.25H0V6.75Z"
              fill="#282938"
            />
          </svg>
        </router-link>
      </div>

      <div class="grid md:grid-cols-3 grid-cols-1 gap-4 pt-10 mb-[60px] md:mb-[100px]">
        <div class="overflow-hidden group relative md:col-span-2 md:mb-[64px]">
          <img src="../../public/Card.png" alt="" class="w-full h-full"/>
          <div
            class="md:w-[47%] w-full absolute -left-full group-hover:left-0 duration-500 top-0 h-[100%] bg-our_hover z-10 flex flex-col justify-end pb-5 md:pb-20"
          >
            <div class="">
              <h2 class="md:text-[26px] text-[15px] font-medium md:font-bold md:leading-[36px] text-white mx-5 md:mx-11">
                Workhub office Webflow Webflow Design
              </h2>
              <p
                class="opacity-[80%] md:text-[18px] md:font-bold ms:leading-[28px] mt-2 md:mt-5 text-white mx-5 md:mx-11 text-[12px]"
              >
                Euismod faucibus turpis eu gravida mi. Pellentesque et velit
                aliquam
              </p>
              <button
                class="text-[#FCD980] mx-5 mt-4 md:mx-11 md:mt-10 flex gap-2 items-center text-[13px] md:text-[20px]"
              >
                <span>View project</span>
                <svg
                  width="25"
                  height="12"
                  viewBox="0 0 25 12"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M24.5303 6.53033C24.8232 6.23744 24.8232 5.76256 24.5303 5.46967L19.7574 0.696699C19.4645 0.403806 18.9896 0.403806 18.6967 0.696699C18.4038 0.989593 18.4038 1.46447 18.6967 1.75736L22.9393 6L18.6967 10.2426C18.4038 10.5355 18.4038 11.0104 18.6967 11.3033C18.9896 11.5962 19.4645 11.5962 19.7574 11.3033L24.5303 6.53033ZM0 6.75H24V5.25H0V6.75Z"
                    fill="#FCD980"
                  />
                </svg>
              </button>
            </div>
          </div>
        </div>

        <div>
          <div class="relative ml-2 overflow-hidden group mb-[37px]">
            <img class="w-[100%]" src="../../public/Card3.png" alt="" />
            <div
              class="w-[100%] absolute -left-full duration-500 group-hover:left-0 top-0 h-[100%] bg-our_hover z-10 flex flex-col justify-end p-10"
            >
              <h1 class="text-[26px] font-bold leading-[36px] text-white mx-11">
                Unisaas Website Design
              </h1>
              <button class="text-[#FCD980] mx-11 mt-4 flex gap-2 items-center">
                <span>View portfolio</span>
                <svg
                  width="25"
                  height="12"
                  viewBox="0 0 25 12"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M24.5303 6.53033C24.8232 6.23744 24.8232 5.76256 24.5303 5.46967L19.7574 0.696699C19.4645 0.403806 18.9896 0.403806 18.6967 0.696699C18.4038 0.989593 18.4038 1.46447 18.6967 1.75736L22.9393 6L18.6967 10.2426C18.4038 10.5355 18.4038 11.0104 18.6967 11.3033C18.9896 11.5962 19.4645 11.5962 19.7574 11.3033L24.5303 6.53033ZM0 6.75H24V5.25H0V6.75Z"
                    fill="#FCD980"
                  />
                </svg>
              </button>
            </div>
          </div>

          <div class="relative ml-2 overflow-hidden group">
            <img class="w-[100%]" src="../../public/Card2.png" alt="" />
            <div
              class="w-[100%] absolute -left-full duration-500 group-hover:left-0 top-0 h-[100%] bg-our_hover z-10 flex flex-col justify-end p-10"
            >
              <h1 class="text-[26px] font-bold leading-[36px] text-white mx-11">
                Unisaas Website Design
              </h1>
              <button class="text-[#FCD980] mx-11 mt-4 flex gap-2 items-center">
                <span>View portfolio</span>
                <svg
                  width="25"
                  height="12"
                  viewBox="0 0 25 12"
                  fill="none"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    d="M24.5303 6.53033C24.8232 6.23744 24.8232 5.76256 24.5303 5.46967L19.7574 0.696699C19.4645 0.403806 18.9896 0.403806 18.6967 0.696699C18.4038 0.989593 18.4038 1.46447 18.6967 1.75736L22.9393 6L18.6967 10.2426C18.4038 10.5355 18.4038 11.0104 18.6967 11.3033C18.9896 11.5962 19.4645 11.5962 19.7574 11.3033L24.5303 6.53033ZM0 6.75H24V5.25H0V6.75Z"
                    fill="#FCD980"
                  />
                </svg>
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- end our project -->

  <!-- start features -->
  <section class="bg-features">
    <div class="container pt-[70px] md:pt-[128px] pb-[70px] md:pb-[128px] px-5 md:px-0">
      <p class="text-center font-medium text-[16px] leading-[28px]">Features</p>
      <div class="w-full flex justify-center mt-[12px]">
        <p
          class="text-center font-semibold text-[20px] md:text-[48px] md:leading-[64px] md:w-[45%] font-[Poppins]"
        >
          Design that solves problems, one product at a time
        </p>
      </div>
      
      <div class="grid md:grid-cols-3 grid-rows-2 mt-[47px] gap-[32px]">
        <div
          v-for="(item, index) in column"
          :key="index"
          class="bg-white p-[48px] text-our_project hover:shadow-xl"
        >
          <img :src="item.img" alt="" class="mb-[25px]" />
          <p class="font-normal text-[24px] leading-9 font-[Poppins] mb-3">
            {{ item.title }}
          </p>
          <p class="font-normal text-[16px] leading-7">{{ item.text }}</p>
        </div>
      </div>
    </div>
  </section>
  <!-- end features -->

  <!-- start clients -->
  <div class="temp flex justify-center">
    <div
      class="container max-md:px-[5%] md:grid md:grid-cols-3 gap-[10%] md:mt-[57px] md:py-[128px] py-[64px]"
    >
      <div class="md:col-span-1 col-span-2">
        <h3
          class="md:text-[38px] text-2xl max-md:px-8 md:text-start text-center font-semibold leading-[56px]"
          style="color: rgba(40, 41, 56, 1)"
        >
          What our clients say about us
        </h3>
        <p
          class="md:mt-4 max-md:text-[14px] mt-8"
          style="color: rgba(40, 41, 56, 1)"
        >
          Lorem ipsum dolor sit amet, consectetur adipiscing elit sed.
        </p>
      </div>
      <div class="col-span-2 max-md:mt-8">
        <div class="swiper-container overflow-hidden relative">
          <div class="swiper-wrapper">
            <div
              class="swiper-slide"
              v-for="(testimonial, index) in testimonials"
              :key="index"
            >
              <h5
                class="md:text-[32px] text-[17px] font-medium md:leading-[48px] leading-[30px]"
                style="color: rgba(40, 41, 56, 1)"
              >
                "{{ testimonial.text }}"
              </h5>
              <div class="mt-12 w-full justify-between flex">
                <div class="flex gap-[14px]">
                  <img :src="testimonial.img" alt="testimonial.name" class="w-[52px] h-[52px] rounded-[50%]"/>
                  <div
                    class="flex flex-col justify-start items-center gap-2 max-md:-1"
                  >
                    <h6
                      class="text-[14px] md:text-[18px]"
                      style="color: rgba(40, 41, 56, 1)"
                    >
                      {{ testimonial.name }}
                    </h6>
                    <p
                      class="text-[10px] md:text-[12px]"
                      style="color: rgba(40, 41, 56, 1)"
                    >
                      {{ testimonial.position }}
                    </p>
                  </div>
                </div>
              </div>
            </div>
          </div>
          <div
            class="flex items-center gap-[10px] absolute bottom-0 right-0 z-10"
          >
            <button
              @click="goToPrevSlide"
              class="text-[#282938] md:w-[48px] md:h-[48px] h-[34px] w-[34px] flex items-center justify-center rounded-full hover:bg-[#5239FA] hover:text-white text-xl md:text-4xl"
            >
              &lt;
            </button>
            <button
              @click="goToNextSlide"
              class="md:w-[48px] md:h-[48px] h-[34px] w-[34px] flex items-center justify-center rounded-full text-xl md:text-4xl hover:bg-[#5239FA] hover:text-white"
            >
              &gt;
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>
  <!-- end clients -->

</template>

<script setup>
import { reactive } from "vue";
import icon from "../../public/Icon.png";
import icon2 from "../../public/Icon2.png";
import icon3 from "../../public/Icon3.png";
import { onMounted, ref } from "vue";
import Swiper from "swiper/bundle";
import "swiper/swiper-bundle.css";
const swiper = ref(null);

const column = reactive([
  {
    img: icon,
    title: "Uses Client First",
    text: "Euismod faucibus turpis eu gravida mi. Pellentesque et velit aliquam sed faucib turpis eu gravida mi. Pellentesque et velit aliquam sed mi.",
  },
  {
    img: icon2,
    title: "Two Free Revision Round",
    text: "Euismod faucibus turpis eu gravida mi. Pellentesque et velit aliquam sed faucib turpis eu gravida mi. Pellentesque et velit aliquam sed mi.",
  },
  {
    img: icon3,
    title: "Template Customization",
    text: "Euismod faucibus turpis eu gravida mi. Pellentesque et velit aliquam sed faucib turpis eu gravida mi. Pellentesque et velit aliquam sed mi.",
  },
  {
    img: icon2,
    title: "24/7 Support",
    text: "Euismod faucibus turpis eu gravida mi. Pellentesque et velit aliquam sed faucib turpis eu gravida mi. Pellentesque et velit aliquam sed mi.",
  },
  {
    img: icon3,
    title: "Quick Delivery",
    text: "Euismod faucibus turpis eu gravida mi. Pellentesque et velit aliquam sed faucib turpis eu gravida mi. Pellentesque et velit aliquam sed mi.",
  },
  {
    img: icon,
    title: "Hands-on approach",
    text: "Euismod faucibus turpis eu gravida mi. Pellentesque et velit aliquam sed faucib turpis eu gravida mi. Pellentesque et velit aliquam sed mi.",
  },
]);


const goToPrevSlide = () => {
  swiper.value.slidePrev();
};

const goToNextSlide = () => {
  swiper.value.slideNext();
};

onMounted(() => {
  swiper.value = new Swiper(".swiper-container", {
    loop: true,
    pagination: {
      el: ".swiper-pagination",
    },
  });
});

const testimonials = ref([
  {
    text: "The best agency we’ve worked with so far. They understand our product and are able to add new features focus.",
    img: "/abdulloh2.png",
    name: "Jenny Wilson",
    position: "Vice President",
  },
  {
    text: "The best agency we’ve worked with so far. They understand our product and are able to add new features focus.",
    img: "/about-user3.png",
    name: "John Doe",
    position: "CEO",
  },
  {
    text: "The best agency we’ve worked with so far. They understand our product and are able to add new features focus.",
    img: "/about-user2.png",
    name: "Sarah Smith",
    position: "Marketing Director",
  },
]);
</script>

<style lang="scss" scoped></style>
