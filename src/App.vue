<template>
  <a-layout style="min-height: 100vh">
    <a-layout-sider v-model:collapsed="collapsed" collapsible>
      <a-menu theme="dark" v-model:selectedKeys="selectedKeys" mode="inline">
        <a-menu-item key="1">
          <span>Option 1</span>
        </a-menu-item>
        <a-menu-item key="2">
          <span>Option 2</span>
        </a-menu-item>
      </a-menu>
    </a-layout-sider>
  </a-layout>
</template>
<script lang="ts" setup>
import {ref} from 'vue';
const collapsed = ref(false);
const selectedKeys = ref(['1']);
</script>
<style>
/*:deep(.ant-menu-item,.ant-menu-item-selected) {*/
/*  background-color: red;*/
/*}*/
</style>
