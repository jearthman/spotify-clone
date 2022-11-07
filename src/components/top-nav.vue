<script lang="ts" setup>
import { ref } from "vue";

const avi = ref("galaxybrain.png");
const profileDropdown = ref(false);
</script>

<template>
  <div class="flex w-full justify-between bg-black p-2">
    <div class="flex items-center pl-4">
      <img src="media/spotify.png" class="w-10 rounded-full rotate-180" />
      <span class="text-white text-xl pl-2 font-semibold">Spoofify</span>
    </div>
    <div class="flex items-center">
      <button
        class="
          mr-2
          rounded-full
          border border-transparent
          bg-zinc-800
          p-2
          transition-colors
          text-zinc-300
          hover:text-zinc-50 hover:border-zinc-50
        "
      >
        <mdicon class="text-center" name="home-outline" size="32"></mdicon>
      </button>
      <label
        class="
          flex
          items-center
          rounded-full
          border border-transparent
          bg-zinc-800
          text-zinc-300
          transition-colors
          hover:border-zinc-50 hover:text-zinc-50
          focus-within:border-zinc-50 focus-within:text-zinc-50
        "
      >
        <mdicon
          name="magnify"
          size="24"
          class="m-2 rounded-l-full text-center"
        ></mdicon>
        <input
          type="text"
          class="bg-transparent p-3 pl-0 w-80 text-zinc-50 focus:outline-0"
          placeholder="What do you want to listen to?"
        />
      </label>
    </div>
    <div class="my-auto pr-4">
      <div
        class="
          flex
          bg-zinc-800
          w-fit
          items-center
          rounded-full
          border border-transparent
          transition-colors
          hover:border-zinc-300 hover:cursor-pointer
          action:bg-zinc-700
        "
        @click="profileDropdown = !profileDropdown"
      >
        <img
          :src="'media/avi/' + avi"
          class="w-10 rounded-full border-2 border-transparent"
        />
        <span class="px-2 text-zinc-300">James Earthman</span>
        <mdicon
          :name="profileDropdown ? 'menu-up' : 'menu-down'"
          class="pr-2 text-zinc-300"
        ></mdicon>
      </div>
      <div
        class="
          absolute
          flex flex-col
          bg-zinc-800
          z-10
          mt-2
          rounded-md
          text-zinc-300
          gap-2
          px-2
          py-2
          w-32
          right-6
        "
        v-if="profileDropdown"
      >
        <a href="#" class="pl-1 transition-colors hover:bg-zinc-700 rounded-md"
          >Profile</a
        >
        <a href="#" class="pl-1 transition-colors hover:bg-zinc-700 rounded-md"
          >Settings</a
        >
        <a href="#" class="pl-1 transition-colors hover:bg-zinc-700 rounded-md"
          >Friends</a
        >
        <a href="#" class="pl-1 transition-colors hover:bg-zinc-700 rounded-md"
          >Log out</a
        >
      </div>
    </div>
  </div>
</template>
