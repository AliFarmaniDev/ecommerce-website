<script setup>
import { ref } from 'vue'
import { RouterLink } from 'vue-router'
//importing container layout
import Container from '@/layout/Container.vue'
</script>

<template>
  <header>
    <div class="w-full">
      <Container>
        <div class="flex justify-between  items-center">
          <div class="flex items-center order-2 sm:order-1 mr-[70px] sm:mr-0">
            <!--logo section-->
            <RouterLink to="/">
              <img src="../assets/images/MobileSHOP.CO.png" alt="site logo" class="flex sm:hidden" />
              <img
                src="../assets/images/SHOP.CO.png"
                alt="desctop logo"
                class="hidden sm:flex"
              />
            </RouterLink>
          </div>
          <div class="flex items-center order-1 sm:order-2">
            <nav class=" gap-5 hidden sm:flex items-center">
                <!--router links-->
                <details>
                    <summary>
                        <RouterLink>Shop</RouterLink>
                    </summary>
                </details>
                <RouterLink to="">On Sale</RouterLink>
                <RouterLink to="">New Arrivals</RouterLink>
                <RouterLink to="">Brands</RouterLink>
            </nav>
            <div class="flex sm:hidden">
                <!--mobile menu-->
                <button>
                  <img src="../assets/icons/MobileMenu.png" alt="mobile logo">
                </button>
            </div>
          </div>
          <div class="hidden sm:flex items-center order-3">
            <!--search box-->
            <div class="flex items-center gap-3 w-[370px] h-[35px] bg-[#00000011] px-3 rounded-[20px]">
              <!--dexctop search-->
              <img src="../assets/icons/Vector.png" alt="search icon" class="w-5 h-5">
              <input type="search" value="search here..." class="h-full w-full bg-inherit text-[#00000070]">
            </div>
          </div>
          <div class="flex gap-3 items-center order-3">
            <!--regester-->
            <img src="../assets/icons/Search.png" alt="search icond" class="flex sm:hidden">
            <img src="../assets/icons/Shop.png" alt="shop icon" class="">
            <img src="../assets/icons/Porofile.png" alt="user profile icon" class="">
          </div>
        </div>
      </Container>
    </div>
  </header>
</template>
