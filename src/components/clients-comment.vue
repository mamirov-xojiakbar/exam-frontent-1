<template>
  <div class="w-3/4 pl-[120px] pr-3">
    <h2 class="leading-[48px] text-[36px] text-[#282938] font-medium">
      {{ clientsComment[id].text }}
    </h2>
    <div class="flex justify-between items-center pt-10 pb-20">
      <div class="flex gap-4 items-center">
        <img :src="clientsComment[id].image" alt="" class="w-[52px] rounded-[50%]"/>
        <div>
          <h3 class="leading-[32px] text-[20px] text-[#282938]">
            {{ clientsComment[id].fullName }}
          </h3>
          <p class="leading-[28px] text-[16px] text-[#282938]">
            {{ clientsComment[id].position }}
          </p>
        </div>
      </div>

      <div class="flex gap-2 items-center">
    <button
      :class="
        id == 0
          ? 'p-3 rounded-[50%] bg-white text-black' // 1-chi button
          : 'p-3 rounded-[50%] bg-[#5239FA] text-white' // 2-chi button
      "
      @click="previous"
      id="previousButton"
    >
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="1em"
        height="1em"
        viewBox="0 0 15 15"
      >
        <path
          fill="none"
          :stroke="id == 0 ? 'black' : 'white'" 
          stroke-linecap="square"
          d="M10 14L3 7.5L10 1"
        />
      </svg>
    </button>

    <button
      :class="
        id != 0
          ? 'p-3 rounded-[50%] bg-white text-black'  
          : 'p-3 rounded-[50%] bg-[#5239FA] text-white'  
      "
      @click="next"
      id="nextButton"
    >
      <svg
        xmlns="http://www.w3.org/2000/svg"
        width="1em"
        height="1em"
        viewBox="0 0 15 15"
      >
        <path
          fill="none"
          :stroke="id != 0 ? 'black' : 'white'"
          stroke-linecap="square"
          d="m5 14l7-6.5L5 1"
        />
      </svg>
    </button>
</div>

    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";

const clientsComment = [
  {
    text: '"The best agency we’ve worked with so far. They understand our product and are able to add new features with a great focus."',
    fullName: "Jenny Wilson",
    position: "Vice President",
    image: "mask.png",
  },
  {
    text: '"Biz hozirgacha ishlagan eng yaxshi agentlik. Ular bizning mahsulotimizni tushunishadi va katta etibor bilan yangi xususiyatlarni qoshishga qodir."',
    fullName: "Abdulloh aka",
    position: "Vice President",
    image: "abdulloh2.png",
  },
];

const id = ref(0);

const next = () => {
  if (id.value < clientsComment.length - 1) {
    id.value++;
  }
};

const previous = () => {
  if (id.value > 0) {
    id.value--;
  }
};
</script>

<style scoped>
#nextIcon {
  fill: #000;
}

#nextButton:hover #nextIcon {
  fill: #fff;
}
</style>
