<script lang="ts" setup>
import RouteList from "./route-list.vue";
</script>

<template>
  <div
    class="
      flex flex-col
      gap-4
      flex-grow
      bg-black
      w-1/5
      h-full
      text-zinc-50
      pt-4
      pl-6
    "
  >
    <div
      class="
        flex
        items-center
        opacity-80
        transition-opacity
        hover:cursor-pointer hover:opacity-100
      "
    >
      <mdicon class="text-center" name="library-shelves" size="24"></mdicon>
      <a class="pl-2">Your Library</a>
    </div>
    <div
      class="
        flex
        items-center
        opacity-80
        transition-opacity
        hover:cursor-pointer hover:opacity-100
      "
    >
      <mdicon
        class="text-center text-sky-400"
        name="plus-box"
        size="24"
      ></mdicon>
      <a class="pl-2">Create a Playlist</a>
    </div>
    <div
      class="
        flex
        items-center
        opacity-80
        transition-opacity
        hover:cursor-pointer hover:opacity-100
      "
    >
      <mdicon
        class="text-center text-purple-400"
        name="heart-circle"
        size="24"
      ></mdicon>
      <a class="pl-2">Liked Songs</a>
    </div>
    <div
      class="
        flex
        items-center
        opacity-80
        transition-opacity
        hover:cursor-pointer hover:opacity-100
      "
    >
      <mdicon
        class="text-center text-emerald-400"
        name="bookmark-box"
        size="24"
      ></mdicon>
      <a class="pl-2">Your Episodes</a>
    </div>
    <div class="h-px bg-zinc-700 mr-6"></div>
    <RouteList />
  </div>
</template>
