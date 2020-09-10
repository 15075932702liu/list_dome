<template>
  <div id="app">
    <van-collapse v-model="activeNames" class="van">
      <van-collapse-item title="标题1" name="1">内容</van-collapse-item>
      <van-collapse-item title="标题2" name="2">内容</van-collapse-item>
      <van-collapse v-model="activeNames" title="标题33">
         <van-collapse-item title="标题3" name="3" disabled>内容</van-collapse-item>
      </van-collapse>
    </van-collapse>
  </div>
</template>

<script>

export default {
 data() {
    return {
      activeNames: ['1'],
    };
  },
};
</script>

<style>
   .van{
     width: 100px;
     height: 60px;
   }
</style>
