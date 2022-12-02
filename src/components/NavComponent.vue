<template>
  <div
    class="fixed top-0 mx-auto flex h-[80px] w-full items-center justify-between bg-black p-2 sm:p-5 md:h-[120px] md:px-[25px] md:py-5 lg:h-[140px]">
    <div>
      <RouterLink to="/">
        <img
          class="h-[60px] md:h-[80px] lg:h-[100px]"
          src="../assets/svgs/edclogo.svg"
          alt="" />
      </RouterLink>
    </div>
    <div
      class="hidden pr-0 text-[14px] font-semibold uppercase text-white md:grid md:h-full md:grid-cols-1">
      <div class="flex self-end">
        <div
          class="sm:text-[14px] sm:font-semibold lg:text-[16px] lg:font-bold">
          <RouterLink to="/events"> view events </RouterLink>
          <span class="line sm:px-[10px] lg:px-[15px]">|</span>
          <RouterLink to="/photogallery"> gallery </RouterLink>
          <span class="line sm:px-[10px] lg:px-[15px]">|</span>
          <a href="https://www.edcweek.com/edcweek2021/" target="_blank">
            archive
          </a>
          <span class="line sm:px-[10px] lg:px-[15px]">|</span>
          <a href="https://lasvegas.electricdaisycarnival.com/travel/hotels/" target="_blank">
            hotels
          </a>
          <span class="line sm:px-[10px] lg:px-[15px]">|</span>
          <a href="https://lasvegas.electricdaisycarnival.com/" target="_blank">
            edc las vegas
          </a>
        </div>
      </div>
    </div>
    <div class="flex md:hidden">
      <DropDownComponent />
    </div>
  </div>
</template>

<script>
import { RouterLink, RouterView } from 'vue-router';
import DropDownComponent from './DropDownComponent.vue';
export default {
  components: {
    DropDownComponent
  }
};
</script>

<style scoped>
.line {
  color: #1da5fb;
}
</style>
