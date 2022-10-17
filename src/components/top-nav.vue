<template>
  <div class="flex w-full justify-between bg-black p-2">
    <div class="my-auto">
      <img src="media/spotify.png" class="w-10 rounded-full rotate-180" />
    </div>
    <div class="flex items-center">
      <button
        class="
          mr-2
          rounded-full
          border border-transparent
          bg-slate-800
          p-2
          text-slate-300
          hover:text-slate-100 hover:border-slate-300
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
          bg-slate-800
          text-slate-300
          hover:border-slate-300 hover:text-slate-100
          focus-within:border-slate-300 focus-within:text-slate-100
        "
      >
        <mdicon
          name="magnify"
          size="24"
          class="m-2 rounded-l-full text-center"
        ></mdicon>
        <input
          type="text"
          class="bg-transparent p-3 pl-0 w-80 text-slate-300 focus:outline-0"
          placeholder="What do you want to listen to?"
        />
      </label>
    </div>
    <div class="my-auto">
      <div
        class="
          flex
          bg-slate-800
          w-fit
          items-center
          rounded-full
          border border-transparent
          hover:border-slate-300 hover:cursor-pointer
          action:bg-slate-700
        "
        @click="profileDropdown = !profileDropdown"
      >
        <img
          :src="'media/avi/' + avi"
          class="w-10 rounded-full border-2 border-transparent"
        />
        <span class="px-2 text-slate-300">James Earthman</span>
        <mdicon
          :name="profileDropdown ? 'menu-up' : 'menu-down'"
          class="pr-2 text-slate-300"
        ></mdicon>
      </div>
      <div
        class="
          absolute
          flex flex-col
          bg-slate-800
          z-10
          mt-2
          rounded-md
          text-slate-300
          gap-2
          px-2
          py-2
          w-32
          right-2
        "
        v-if="profileDropdown"
      >
        <a href="#" class="pl-1 hover:bg-slate-700 rounded-md">Profile</a>
        <a href="#" class="pl-1 hover:bg-slate-700 rounded-md">Settings</a>
        <a href="#" class="pl-1 hover:bg-slate-700 rounded-md">Friends</a>
        <a href="#" class="pl-1 hover:bg-slate-700 rounded-md">Log out</a>
      </div>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  name: "TopNav",
  data() {
    return {
      avi: "galaxybrain.png",
      profileDropdown: false,
    };
  },
};
</script>
