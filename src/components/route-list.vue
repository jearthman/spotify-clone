<template>
  <div>
    <ul>
      <li v-for="route in routes" @click="">{{route.name}}</li>
    </ul>
  </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue';

interface Route{
  type: string, 
  id: string, 
  name: string
}

export default defineComponent({
  name: "RouteList",
  props: {
    routes: Array<Route>
  },
  data() {
    return {
    }
  },
})
</script>