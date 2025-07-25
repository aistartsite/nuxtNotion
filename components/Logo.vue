<template>
  <svg 
    :class="sizeClass" 
    viewBox="0 0 24 24"
    :style="{ cursor: clickable ? 'pointer' : 'default' }"
    @click="handleClick"
  >
    <defs>
      <linearGradient :id="gradientId" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" style="stop-color:#667eea;stop-opacity:1" />
        <stop offset="50%" style="stop-color:#764ba2;stop-opacity:1" />
        <stop offset="100%" style="stop-color:#f093fb;stop-opacity:1" />
      </linearGradient>
    </defs>
    <path 
      :fill="`url(#${gradientId})`"
      d="M4.459 4.208c.746.606 1.026.56 2.428.466l13.215-.793c.28 0 .047-.28-.046-.326L17.86 1.968c-.42-.326-.981-.7-2.055-.607L3.01 2.295c-.466.046-.56.28-.374.466zm.793 3.08v13.904c0 .747.373 1.027 1.214.98l14.523-.84c.841-.046.935-.56.935-1.167V6.354c0-.606-.233-.933-.748-.887l-15.177.887c-.56.047-.747.327-.747.933zm14.337.745c.093.42 0 .84-.42.888l-.7.14v10.264c-.608.327-1.168.514-1.635.514-.748 0-.935-.234-1.495-.933l-4.577-7.186v6.952L12.21 19s0 .84-1.168.84l-3.222.186c-.093-.186 0-.653.327-.746l.84-.233V9.854L7.822 9.76c-.094-.42.14-1.026.793-1.073l3.456-.233 4.764 7.279v-6.44l-1.215-.139c-.093-.514.28-.887.747-.933zM1.936 1.035l13.31-.98c1.634-.14 2.055-.047 3.082.7l4.249 2.986c.7.513.934.747.934 1.213v16.378c0 1.026-.373 1.634-1.68 1.726l-15.458.934c-.98.047-1.448-.093-1.962-.747l-3.129-4.06c-.56-.747-.793-1.306-.793-1.96V2.667c0-.839.374-1.54 1.447-1.632z" 
    />
  </svg>
</template>

<script setup>
import { computed, ref } from 'vue'

// 定义 props
const props = defineProps({
  // 尺寸预设
  size: {
    type: String,
    default: 'md',
    validator: (value) => ['xs', 'sm', 'md', 'lg', 'xl', '2xl'].includes(value)
  },
  // 自定义类名
  customClass: {
    type: String,
    default: ''
  },
  // 是否可点击
  clickable: {
    type: Boolean,
    default: false
  }
})

// 定义事件
const emit = defineEmits(['click'])

// 生成唯一的渐变 ID，避免多个组件实例之间的冲突
const gradientId = ref(`notionGradient-${Math.random().toString(36).substr(2, 9)}`)

// 计算尺寸类名
const sizeClass = computed(() => {
  const sizeMap = {
    'xs': 'w-4 h-4',
    'sm': 'w-6 h-6',
    'md': 'w-8 h-8',
    'lg': 'w-10 h-10',
    'xl': 'w-12 h-12',
    '2xl': 'w-16 h-16'
  }
  
  const baseClass = sizeMap[props.size] || sizeMap.md
  return props.customClass ? `${baseClass} ${props.customClass}` : baseClass
})

// 处理点击事件
const handleClick = () => {
  if (props.clickable) {
    emit('click')
  }
}
</script>

<style scoped>
/* 可以添加一些基础的过渡效果 */
svg {
  transition: transform 0.2s ease-in-out;
}

svg:hover {
  transform: scale(1.05);
}
</style>