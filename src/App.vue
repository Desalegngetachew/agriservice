<script setup>
import { RouterLink, RouterView } from "vue-router";
</script>

<template>
  <header>
    <div class="w-full">
      <nav class="flex py-3 items-center bg-gray-50 pl-5 shadow-lg">
        <div class="flex">
          <router-link to="/"
            ><img src="./assets/logo.jpg" class="h-10 w-10"
          /></router-link>
        </div>
        <div class="flex items-center w-[100%] justify-end gap-x-12">
          <div class="flex gap-5 w-fit">
            <RouterLink to="/">መነሻ</RouterLink>
            <RouterLink to="/product">ውጤቶች</RouterLink>
            <RouterLink to="/store">መደብር</RouterLink>
            <RouterLink to="/event">ክስተቶች</RouterLink>
            <RouterLink to="/about">ስለኛ</RouterLink>
          </div>
          <div class="flex w-fit gap-3 px-5">
            <RouterLink to="/cart"
              ><svg
                class="fill-current text-blue-900 w-5 h-5"
                focusable="false"
                aria-hidden="true"
                viewBox="0 0 24 24"
                data-testid="ShoppingCartIcon"
                tabindex="-1"
                title="ShoppingCart"
              >
                <path
                  d="M7 18c-1.1 0-1.99.9-1.99 2S5.9 22 7 22s2-.9 2-2-.9-2-2-2zM1 2v2h2l3.6 7.59-1.35 2.45c-.16.28-.25.61-.25.96 0 1.1.9 2 2 2h12v-2H7.42c-.14 0-.25-.11-.25-.25l.03-.12.9-1.63h7.45c.75 0 1.41-.41 1.75-1.03l3.58-6.49c.08-.14.12-.31.12-.48 0-.55-.45-1-1-1H5.21l-.94-2H1zm16 16c-1.1 0-1.99.9-1.99 2s.89 2 1.99 2 2-.9 2-2-.9-2-2-2z"
                ></path></svg
            ></RouterLink>
            <RouterLink to="/auth"
              ><svg
                class="fill-current text-blue-900 w-5 h-5"
                focusable="false"
                aria-hidden="true"
                viewBox="0 0 24 24"
                data-testid="PersonOutlineIcon"
                tabindex="-1"
                title="PersonOutline"
              >
                <path
                  d="M12 5.9c1.16 0 2.1.94 2.1 2.1s-.94 2.1-2.1 2.1S9.9 9.16 9.9 8s.94-2.1 2.1-2.1m0 9c2.97 0 6.1 1.46 6.1 2.1v1.1H5.9V17c0-.64 3.13-2.1 6.1-2.1M12 4C9.79 4 8 5.79 8 8s1.79 4 4 4 4-1.79 4-4-1.79-4-4-4zm0 9c-2.67 0-8 1.34-8 4v3h16v-3c0-2.66-5.33-4-8-4z"
                ></path></svg
            ></RouterLink>
          </div>
        </div>
      </nav>
    </div>
  </header>

  <RouterView />
  
</template>

<style scoped>
@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }
}
</style>
