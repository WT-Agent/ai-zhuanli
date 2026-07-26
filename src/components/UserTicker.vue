<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 138****2211 完成了 AI 模型压缩算法发明专利交底书"
  },
  {
    "text": "用户 189****9900 获得了机械传动结构实用新型交底书草案"
  },
  {
    "text": "用户 131****4455 完成了权利要求书独立与从属权利布局"
  },
  {
    "text": "用户 156****7788 生成了专利审查意见通知书 (OA) 答辩策略"
  },
  {
    "text": "用户 173****3311 取得了交底书附图标记与具体实施例 Checklist"
  }
]);
</script>
