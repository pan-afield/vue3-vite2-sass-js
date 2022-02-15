<script setup>
import { onMounted, ref } from "vue";
import { useStore } from 'vuex'
defineProps({
  msg: String,
});
const count = ref(0);
const store = useStore()
console.log(store.state.num);
onMounted(() => {
  console.log('渲染完成');
})
</script>

<template>
  <div>Home</div>
  <div></div>
  <van-button type="primary">主要按钮</van-button>
</template>

<style lang="scss" scoped>
</style>
