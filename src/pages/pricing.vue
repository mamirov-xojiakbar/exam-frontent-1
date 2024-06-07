<template>
  <!-- start Our Pricing Plans -->
  <section class="container pt-[120px] md:pt-[200px] px-5 md:px-0">
    <div class="w-full text-center md:px-[380px]">
      <p class="text-[Poppins] font-semibold text-[30px] md:text-[48px] md:leading-[64px] mb-4">
        Our Pricing Plans
      </p>
      <p class="opacity-[70%] font-medium text-[16px] md:leading-[28px]">
        When you’re ready to go beyond prototyping in Figma, Webflow is ready to
        help you bring your designs to life — without coding them.
      </p>
    </div>

    <div class="grid md:grid-cols-3 gap-[32px] mt-[64px] mb-[128px]">
      <div
        v-for="(item, index) in arr"
        :key="index"
        :class="item.id == 2 ? 'bg-tint_blue text-white' : 'bg-features'"
        class="py-[64px] px-[48px] rounded-3xl relative overflow-hidden"
      >
        <div
            v-if="index == 1"
            class="z-10 w-[1000px] h-[1000px] rounded-full absolute top-[10%] md:top-[12%] left-1/2 -translate-x-1/2 -translate-y-1/2 bg-white opacity-[6%]"
        ></div>

        <div class="flex items-center gap-2 mb-5">
          <p class="font-[Poppins] font-semibold text-[38px] leading-[56px]">
            {{ item.price }}
          </p>
          <a
            href="#"
            class="font-normal"
            :class="item.id == 2 ? 'text-[#FCD980]' : 'text-[#2405F2]'"
            >{{ item.type }}</a
          >
        </div>

        <p class="font-[Poppins] font-medium text-[24px] leading-[36px]">
          {{ item.title }}
        </p>

        <p
          class="font-medium text-[16px] leading-[28px] mt-2 opacity-[70%] mb-[50px]"
        >
          {{ item.text }}
        </p>

        <div
          v-for="(i, index) in item.column"
          :key="index"
          class="flex items-center gap-3"
        >
          <img src="../../public/Pointer.png" alt="" class="mb-5" />
          <a
            href="#"
            class="font-normal text-4 leading-[28px]"
            :class="item.id == 2 ? 'mb-4' : 'mb-5'"
            >{{ i }}</a
          >
        </div>

        <div class="w-full flex justify-center mt-[76px]">
          <router-link
            to=""
            class="font-semibold text-[18px] leading-[32px] py-4 px-[50px] md:px-[77px] rounded-[41px]"
            :class="
              item.id == 2
                ? 'bg-[#FCD980] text-black'
                : 'bg-[#282938] text-white'
            "
          >
            {{ item.button }}
          </router-link>
        </div>
      </div>
    </div>
  </section>
  <!-- end Our Pricing Plans -->

  <!-- start Frequently -->
  <section class="container px-5 md:px-0">
    <div class="md:flex mb-[128px]">
      <div class="md:w-[35%] mb-10 md:mb-0">
        <p
          class="font-[Poppins] font-semibold text-[30px] md:text-[40px] md:leading-[64px] mb-4"
        >
          Frequently asked questions
        </p>

        <a href="#" class="text-[#2405F2]">Contact us For More Info</a>
      </div>

      <div>
        <div
          class="border-b-[1px] border-b-[#C2BBFFB2] py-4"
          v-for="(item, index) in arr2"
          :key="index"
        >
          <button
            class="w-full text-left flex justify-between items-center cursor-pointer font-[Poppins] font-normal md:text-[20px]"
            @click="toggleFAQ(index)"
          >
            <div class="text-[#2405F2] font-bold">0{{ index + 1 }}</div>
            <div class="ml-4 flex-1">{{ item.question }}</div>
            <div>
              <template v-if="item.open">
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="1.5em"
                  height="1.5em"
                  viewBox="0 0 24 24"
                >
                  <path
                    fill="black"
                    d="M19 6.41L17.59 5L12 10.59L6.41 5L5 6.41L10.59 12L5 17.59L6.41 19L12 13.41L17.59 19L19 17.59L13.41 12z"
                  />
                </svg>
              </template>

              <template v-else>
                <svg
                  xmlns="http://www.w3.org/2000/svg"
                  width="1.5em"
                  height="1.5em"
                  viewBox="0 0 24 24"
                >
                  <path
                    fill="black"
                    d="M18 12.998h-5v5a1 1 0 0 1-2 0v-5H6a1 1 0 0 1 0-2h5v-5a1 1 0 0 1 2 0v5h5a1 1 0 0 1 0 2"
                  />
                </svg>
              </template>
            </div>
          </button>

          <div
            class="mt-4 faq-item"
            :class="{ open: item.open, closed: !item.open }"
          >
            <p class="text-gray-700 ml-10">{{ item.answer }}</p>
          </div>
        </div>
      </div>
    </div>
  </section>
  <!-- end Frequently -->
</template>

<script setup>
import { reactive } from "vue";

const arr = reactive([
  {
    id: 1,
    price: "$299",
    type: "Per Design",
    title: "Landing Page",
    text: "When you’re ready to go beyond prototyping in Figma,",
    column: [
      "All limited links",
      "Own analytics platform",
      "Chat support",
      "Optimize hashtags",
      "Unlimited users",
    ],
    button: "Get started",
  },
  {
    id: 2,
    price: "$399",
    type: "Multi Design",
    title: "Website Page",
    text: "When you’re ready to go beyond prototyping in Figma, Webflow’s ready to help.",
    column: [
      "All limited links",
      "Own analytics platform",
      "Chat support",
      "Optimize hashtags",
      "Unlimited users",
    ],
    button: "Get started",
  },
  {
    id: 3,
    price: "$499 +",
    type: "Per Design",
    title: "Complex Project",
    text: "When you’re ready to go beyond prototyping in Figma,",
    column: [
      "All limited links",
      "Own analytics platform",
      "Chat support",
      "Optimize hashtags",
      "Unlimited users",
    ],
    button: "Contact us",
  },
]);

const arr2 = reactive([
  {
    question: "How much time does it take?",
    answer:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.",
    open: true,
  },
  {
    question: "What is your class naming convention?",
    answer: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
    open: false,
  },
  {
    question: "How do we communicate?",
    answer: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
    open: false,
  },
  {
    question: "I have a bigger project. Can you handle it?",
    answer: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
    open: false,
  },
  {
    question: "What is your class naming convention?",
    answer: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
    open: false,
  },
]);

function toggleFAQ(index) {
  this.arr2[index].open = !this.arr2[index].open;
}
</script>

<style scoped>
.faq-item {
  transition: max-height 0.3s ease;
}
.faq-item.closed {
  max-height: 0;
  overflow: hidden;
}
.faq-item.open {
  max-height: 500px;
}
</style>
