<template>
  <div class="flex w-full justify-between bg-black p-2">
    <div>TEST</div>
    <div class="flex items-center">
      <button
        class="
          mr-2
          rounded-full
          border border-transparent
          bg-slate-800
          p-2
          text-slate-300
          hover:text-slate-100
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
          focus:border-slate-300 focus:text-slate-100
        "
      >
        <mdicon
          name="magnify"
          size="24"
          class="m-2 rounded-l-full text-center"
        ></mdicon>
        <input
          type="text"
          class="
            bg-transparent
            p-3
            pl-0
            text-slate-300
            focus:border-slate-300 focus:outline-0
          "
        />
      </label>
    </div>
    <div>TEST2</div>
  </div>
</template>

<script lang="ts">
export default {
  name: "TopNav",
  data() {
    return {};
  },
};
</script>
