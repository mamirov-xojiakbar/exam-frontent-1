<template>
  <section class="container pt-[130px] md:pt-[190px] text-center pb-[60px] md:pb-[128px] px-5 md:px-0">
    <div class="w-full flex justify-center mb-[16px]">
        <p class="font-[Poppins] font-semibold md:text-[48px] md:leading-[64px] w-[70%]">
            A UX Case Study on Creating a Studious Environment for Students
        </p>
    </div>

    <p class="font-[Poppins] font-medium text-[16px] leading-[28px] mb-[32px]">
        Andrew Jonson Posted on 27th January 2021
    </p>

    <img src="../../public/blog1.png" alt="" class="w-full mb-[48px]"/>
    
    <div class="flex justify-center w-full mb-[16px]">
        <p class="font-[Poppins] font-normal text-[13px] md:text-[16px] leading-[28px] md:w-[65%] opacity-[70%]">
          Apparently we had reached a great height in the atmosphere, for the sky
          was a dead black, and the stars had ceased to twinkle. By the same
          illusion which lifts the horizon of the sea to the level of the spectator
          on a hillside.
        </p>
    </div>
    
    <a href="#" class="font-[Poppins] font-normal text-[16px] leading-[28px] w-[65%] text-[#2405F2]">
        Read more
    </a>
  </section>

  <section class="container pb-[40px] md:pb-[128px] px-5 md:px-0">
    <p class="font-[Poppins] font-semibold text-center text-[30px] md:text-[48px] leading-[64px] mb-[48px]">
        Our Blog
    </p>
    <div class="md:grid grid-cols-3 gap-[22px]">
        <div v-for="item, index in blog" :key="index" class="mb-5 md:mb-0 hover:shadow-lg p-5 pb-10">
            <img :src="item.img" alt="" class="w-full">
            <p class="font-[Poppins] font-medium text-[16px] leading-[28px] opacity-[70%] mt-[32px] mb-[16px]">{{ item.date }}</p>
            <p class="font-[Poppins] font-normal text-[24px] leading-[36px] mb-[16px]">{{ item.title }}</p>
            <p class="font-[Poppins] font-normal text-[16px] leading-[28px] opacity-[70%] mb-[24px]">{{ item.text }}</p>
            <router-link to="#" class="flex items-center gap-3 font-[Poppins] font-normal text-[16px] leading-[28px]">
                Read More
                <img src="../../public/Arrow3.png" alt="">
            </router-link>
        </div>
    </div>
  </section>
</template>

<script setup>
import { reactive } from 'vue';
import img1 from "../../public/our1.png"
import img2 from "../../public/our2.png"
import img3 from "../../public/our3.png"
import img4 from "../../public/our4.png"
import img5 from "../../public/our5.png"
import img6 from "../../public/our6.png"

const blog = reactive([
    {
        id: 1,
        img: img1,
        date: "27 Jan 2021",
        title: "How one Webflow user grew his single person consultancy from $0-100K in 14 months",
        text: "See how pivoting to Webflow changed one person’s sales strategy and allowed him to attract"
    },
    {
        id: 2,
        img: img2,
        date: "27 Jan 2021",
        title: "How one Webflow user grew his single person consultancy from $0-100K in 14 months",
        text: "See how pivoting to Webflow changed one person’s sales strategy and allowed him to attract"
    },
    {
        id: 3,
        img: img3,
        date: "27 Jan 2021",
        title: "How one Webflow user grew his single person consultancy from $0-100K in 14 months",
        text: "See how pivoting to Webflow changed one person’s sales strategy and allowed him to attract"
    },
    {
        id: 4,
        img: img4,
        date: "27 Jan 2021",
        title: "How one Webflow user grew his single person consultancy from $0-100K in 14 months",
        text: "See how pivoting to Webflow changed one person’s sales strategy and allowed him to attract"
    },
    {
        id: 5,
        img: img5,
        date: "27 Jan 2021",
        title: "How one Webflow user grew his single person consultancy from $0-100K in 14 months",
        text: "See how pivoting to Webflow changed one person’s sales strategy and allowed him to attract"
    },
    {
        id: 6,
        img: img6,
        date: "27 Jan 2021",
        title: "How one Webflow user grew his single person consultancy from $0-100K in 14 months",
        text: "See how pivoting to Webflow changed one person’s sales strategy and allowed him to attract"
    }
])
</script>

<style lang="scss" scoped></style>
