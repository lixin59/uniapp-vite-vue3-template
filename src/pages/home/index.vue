<template>
  <view class="content">
    <view style="padding: 20px">
      <u-tag :text="state.tag" plain size="mini" type="warning"></u-tag>
      <u-alert
        :title="state.title"
        type="warning"
        effect="dark"
        :description="state.description"
      ></u-alert>
    </view>
  </view>
</template>

<script setup lang="ts">
  import { reactive } from 'vue';
  const state = reactive({
    title: 'title',
    tag: '测试标签',
    description: 'description',
  });
</script>

<style>
  .content {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
  }

  .logo {
    height: 200rpx;
    width: 200rpx;
    margin-top: 200rpx;
    margin-left: auto;
    margin-right: auto;
    margin-bottom: 50rpx;
  }

  .text-area {
    display: flex;
    justify-content: center;
  }

  .title {
    font-size: 36rpx;
    color: #8f8f94;
  }
</style>
