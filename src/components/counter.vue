<template>
  <div class="h-screen w-screen flex flex-col items-center justify-center gap-10">
    <img
      v-if="isturnon"
      src="../images/turnon-removebg-preview.png"
      class="h-28"
      alt=""
    />
    <img v-else src="../images/turnoff-removebg-preview.png" class="h-28" alt="" />
    <div class="flex gap-4">
      <button
        @click="turnOn"
        class="border border-transparent py-2 px-8 rounded-xl bg-green-500"
        type=""
      >
        Yoqish
      </button>
      <button
        @click="turnOff"
        class="border border-transparent py-2 px-8 rounded-xl bg-red-500"
        type=""
      >
        O'chirish
      </button>
    </div>
  </div>
</template>

<script setup>
import { ref, reactive } from "vue";
let isturnon = ref(false);
function turnOn() {
  isturnon.value = true;
}
function turnOff() {
  isturnon.value = false;
}
</script>

<style scoped></style>
