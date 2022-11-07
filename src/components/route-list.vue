<script lang="ts" setup>
import { defineComponent, PropType } from "vue";

interface Route {
  type: string;
  id: string;
  name: string;
}

const props = defineProps({
  routes: Array as PropType<Array<Route>>,
});
</script>

<template>
  <div>
    test
    <ul>
      <li v-for="route in routes" :key="route.id">{{ route.name }}</li>
    </ul>
  </div>
</template>