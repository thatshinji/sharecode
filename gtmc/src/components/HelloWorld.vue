<script setup lang="ts">
import { Ref, ref } from 'vue'
// props 声明方式
defineProps<{ msg: string }>()

const count = ref(0) // 等同下一行代码
const count2: Ref<number> = ref<number>(1)

</script>

<template>
  <h1>{{ msg }}</h1>
  <div class="card">
    <button type="button" @click="count++">count is {{ count }}</button>
  </div>
</template>

<style scoped>
.read-the-docs {
  color: #888;
}
</style>
<!-- defineComponent 声明方式 -->
<!-- defineComponent({
  props: {
    msg: {
      type: String
      default: ''
    }
  }
}) -->