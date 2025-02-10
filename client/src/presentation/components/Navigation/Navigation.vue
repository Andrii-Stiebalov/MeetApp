<script lang="ts">
import { defineComponent } from 'vue'
export default defineComponent({
  name: 'Navigation',
  data() {
    return {
      navList: [
        {
          name: 'Home',
          icon: 'home',
        },
        {
          name: 'List',
          path: '/list',
          icon: 'search',
        },
        {
          name: 'Profile',
          icon: 'user',
        },
      ],
    }
  },
  methods: {
    goToRoute(path: string) {
      try {
        void this.$router.push(path)
      } catch {
        console.error('')
      }
    },
  },
},
)
</script>

<template>
  <div class="Navigation">
    <div
      v-for="nav in navList"
      :key="nav.name"
      @click="() => goToRoute(nav.path)"
    >
      {{ nav.name }}
    </div>
  </div>
</template>

<style>
.Navigation {
  position: fixed;
  bottom: 0;
  left: 0;
  right: 0;
  display: flex;
  background-color: #fff;
  height: 50px;
  background: green;

  justify-content: space-around;
  align-items: center;
  border-radius: 5px 5px 0 0 ;
  text-transform: uppercase;
}
</style>
