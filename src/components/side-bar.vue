<template>
  <div
    class="
      flex flex-col
      gap-4
      flex-grow
      bg-black
      w-1/5
      h-full
      text-slate-50
      pt-4
    "
  >
    <div
      class="
        flex
        items-center
        pl-4
        opacity-80
        hover:text-slate-50 hover:cursor-pointer hover:opacity-100
      "
    >
      <mdicon class="text-center" name="library-shelves" size="24"></mdicon>
      <a class="pl-2">Your Library</a>
    </div>
    <div
      class="
        flex
        items-center
        pl-4
        opacity-80
        hover:text-slate-50 hover:cursor-pointer hover:opacity-100
      "
    >
      <mdicon
        class="text-center text-green-400"
        name="plus-box"
        size="24"
      ></mdicon>
      <a class="pl-2">Create a Playlist</a>
    </div>
    <div
      class="
        flex
        items-center
        pl-4
        opacity-80
        hover:text-slate-50 hover:cursor-pointer hover:opacity-100
      "
    >
      <mdicon
        class="text-center text-purple-400"
        name="heart-circle"
        size="24"
      ></mdicon>
      <a class="pl-2">Liked Songs</a>
    </div>
  </div>
</template>

<script lang="ts">
export default {
  name: "SideBar",
  data() {
    return {};
  },
};
</script>
