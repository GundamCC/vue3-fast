<template>
  <h2>欢迎使用新时代前端框架</h2>
  <div>{{ userStore.name }}</div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import { useUserStore } from '@/store/user'

export default defineComponent({
  name: 'UsePinia',
  setup() {
    const userStore = useUserStore()

    return {
      userStore,
    }
  },
})
</script>
