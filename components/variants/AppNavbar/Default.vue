<template>
  <nav class="bg-white/95 dark:bg-gray-800/95 backdrop-blur-md shadow-lg border-b border-gray-200 dark:border-gray-700 sticky top-0 z-50 transition-colors duration-300">
    <div class="container mx-auto px-4">
      <div class="flex justify-between items-center min-h-16 py-3 md:py-4">
        <!-- 左侧：Logo + 菜单 -->
        <div class="flex items-center space-x-8">
          <!-- Logo -->
          <NuxtLink to="/" class="flex items-center space-x-3 group">
            <div class="relative">
              <Logo
              size="xs"
              custom-class="w-8 h-8"
              :clickable="true"
            />
              <!-- 悬停时的光晕效果 -->
              <div class="absolute inset-0 w-8 h-8 bg-gradient-to-br from-blue-500/20 to-purple-600/20 rounded-lg opacity-0 group-hover:opacity-100 transition-opacity duration-300 -z-10 blur-sm scale-150"></div>
            </div>
            <h1 class="text-xl md:text-2xl font-bold bg-gradient-to-r from-blue-600 to-purple-600 dark:from-blue-400 dark:to-purple-400 bg-clip-text text-transparent transition-all duration-300 group-hover:from-blue-500 group-hover:to-purple-500">NuxtNotion</h1>
          </NuxtLink>
          
          <!-- 桌面端导航菜单 -->
          <div class="hidden md:flex items-center space-x-6">
            <NuxtLink to="/" class="relative text-gray-600 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 transition-all duration-200 py-2 px-1 group">
              首页
              <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-blue-600 dark:bg-blue-400 transition-all duration-200 group-hover:w-full"></span>
            </NuxtLink>
            <NuxtLink to="/guide" class="relative text-gray-600 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 transition-all duration-200 py-2 px-1 group">
              指南
              <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-blue-600 dark:bg-blue-400 transition-all duration-200 group-hover:w-full"></span>
            </NuxtLink>
            <NuxtLink to="/articles" class="relative text-gray-600 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 transition-all duration-200 py-2 px-1 group">
              文章
              <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-blue-600 transition-all duration-200 group-hover:w-full"></span>
            </NuxtLink>
            <NuxtLink to="/pro" class="relative text-gray-600 dark:text-gray-300 hover:text-orange-600 dark:hover:text-orange-400 transition-all duration-200 py-2 px-1 group">
              <span class="flex items-center space-x-1">
                <span>PRO</span>
                <span class="inline-flex items-center px-1.5 py-0.5 rounded-full text-xs font-medium bg-gradient-to-r from-orange-500 to-red-500 text-white">
                  NEW
                </span>
              </span>
              <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-orange-600 dark:bg-orange-400 transition-all duration-200 group-hover:w-full"></span>
            </NuxtLink>
            <NuxtLink to="/about" class="relative text-gray-600 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 transition-all duration-200 py-2 px-1 group">
              关于
              <span class="absolute bottom-0 left-0 w-0 h-0.5 bg-blue-600 dark:bg-blue-400 transition-all duration-200 group-hover:w-full"></span>
            </NuxtLink>
          </div>
        </div>
        
        <!-- 右侧：功能按钮 -->
        <div class="flex items-center space-x-3">
          <!-- 主题切换按钮 -->
          <button 
            @click="toggleTheme"
            class="hidden md:flex w-10 h-10 items-center justify-center text-gray-600 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 hover:bg-blue-50 dark:hover:bg-gray-700 rounded-lg transition-all duration-200"
            :title="isDark ? '切换到浅色模式' : '切换到深色模式'"
          >
            <svg v-if="isDark" class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 3v1m0 16v1m9-9h-1M4 12H3m15.364 6.364l-.707-.707M6.343 6.343l-.707-.707m12.728 0l-.707.707M6.343 17.657l-.707.707M16 12a4 4 0 11-8 0 4 4 0 018 0z"></path>
            </svg>
            <svg v-else class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M20.354 15.354A9 9 0 018.646 3.646 9.003 9.003 0 0012 21a9.003 9.003 0 008.354-5.646z"></path>
            </svg>
          </button>
          
          <!-- 语言切换按钮（暂时隐藏） -->
          <!-- <button 
            @click="toggleLanguage"
            class="hidden md:flex w-10 h-10 items-center justify-center text-gray-600 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 hover:bg-blue-50 dark:hover:bg-gray-700 rounded-lg transition-all duration-200 text-sm font-medium"
            :title="isEnglish ? '切换到中文' : 'Switch to English'"
          >
            {{ isEnglish ? '中' : 'EN' }}
          </button> -->
          
          <!-- GitHub按钮 -->
          <a 
            href="https://github.com/yourusername/nuxtnotion" 
            target="_blank" 
            rel="noopener noreferrer"
            class="hidden md:flex w-10 h-10 items-center justify-center text-gray-600 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 hover:bg-blue-50 dark:hover:bg-gray-700 rounded-lg transition-all duration-200"
            title="GitHub"
          >
            <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
              <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
            </svg>
          </a>
        </div>
        
        <!-- 移动端菜单按钮 -->
        <div class="md:hidden">
          <button 
            @click="toggleMobileMenu" 
            class="relative w-10 h-10 text-gray-600 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 focus:outline-none focus:ring-2 focus:ring-blue-500 focus:ring-opacity-50 rounded-lg transition-all duration-200"
            :class="{ 'text-blue-600 dark:text-blue-400': mobileMenuOpen }"
          >
            <span class="sr-only">打开菜单</span>
            <div class="absolute left-1/2 top-1/2 transform -translate-x-1/2 -translate-y-1/2">
              <span 
                class="block w-5 h-0.5 bg-current transform transition-all duration-200"
                :class="mobileMenuOpen ? 'rotate-45 translate-y-1' : '-translate-y-1'"
              ></span>
              <span 
                class="block w-5 h-0.5 bg-current transition-all duration-200"
                :class="mobileMenuOpen ? 'opacity-0' : 'opacity-100'"
              ></span>
              <span 
                class="block w-5 h-0.5 bg-current transform transition-all duration-200"
                :class="mobileMenuOpen ? '-rotate-45 -translate-y-1' : 'translate-y-1'"
              ></span>
            </div>
          </button>
        </div>
      </div>
      
      <!-- 移动端菜单 -->
      <div 
        class="md:hidden overflow-hidden transition-all duration-300 ease-in-out"
        :class="mobileMenuOpen ? 'max-h-96 opacity-100' : 'max-h-0 opacity-0'"
      >
        <div class="py-4 space-y-1">
          <NuxtLink 
            to="/" 
            @click="closeMobileMenu"
            class="block py-2 md:py-3 px-3 md:px-4 text-gray-600 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 hover:bg-blue-50 dark:hover:bg-gray-700 transition-all duration-200 rounded-lg mx-2"
          >
            <div class="flex items-center space-x-3">
              <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 12l2-2m0 0l7-7 7 7M5 10v10a1 1 0 001 1h3m10-11l2 2m-2-2v10a1 1 0 01-1 1h-3m-6 0a1 1 0 001-1v-4a1 1 0 011-1h2a1 1 0 011 1v4a1 1 0 001 1m-6 0h6"></path>
              </svg>
              <span>首页</span>
            </div>
          </NuxtLink>
          <NuxtLink 
            to="/guide" 
            @click="closeMobileMenu"
            class="block py-2 md:py-3 px-3 md:px-4 text-gray-600 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 hover:bg-blue-50 dark:hover:bg-gray-700 transition-all duration-200 rounded-lg mx-2"
          >
            <div class="flex items-center space-x-3">
              <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6.253v13m0-13C10.832 5.477 9.246 5 7.5 5S4.168 5.477 3 6.253v13C4.168 18.477 5.754 18 7.5 18s3.332.477 4.5 1.253m0-13C13.168 5.477 14.754 5 16.5 5c1.747 0 3.332.477 4.5 1.253v13C19.832 18.477 18.247 18 16.5 18c-1.746 0-3.332.477-4.5 1.253"></path>
              </svg>
              <span>指南</span>
            </div>
          </NuxtLink>
          <NuxtLink 
            to="/articles" 
            @click="closeMobileMenu"
            class="block py-2 md:py-3 px-3 md:px-4 text-gray-600 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 hover:bg-blue-50 dark:hover:bg-gray-700 transition-all duration-200 rounded-lg mx-2"
          >
            <div class="flex items-center space-x-3">
              <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12h6m-6 4h6m2 5H7a2 2 0 01-2-2V5a2 2 0 012-2h5.586a1 1 0 01.707.293l5.414 5.414a1 1 0 01.293.707V19a2 2 0 01-2 2z"></path>
              </svg>
              <span>文章</span>
            </div>
          </NuxtLink>
          <NuxtLink 
            to="/pro" 
            @click="closeMobileMenu"
            class="block py-2 md:py-3 px-3 md:px-4 text-gray-600 dark:text-gray-300 hover:text-orange-600 dark:hover:text-orange-400 hover:bg-orange-50 dark:hover:bg-gray-700 transition-all duration-200 rounded-lg mx-2"
          >
            <div class="flex items-center space-x-3">
              <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 3v4M3 5h4M6 17v4m-2-2h4m5-16l2.286 6.857L21 12l-5.714 2.143L13 21l-2.286-6.857L5 12l5.714-2.143L13 3z"></path>
              </svg>
              <span class="flex items-center space-x-2">
                <span>PRO</span>
                <span class="inline-flex items-center px-1.5 py-0.5 rounded-full text-xs font-medium bg-gradient-to-r from-orange-500 to-red-500 text-white">
                  NEW
                </span>
              </span>
            </div>
          </NuxtLink>
          <NuxtLink 
            to="/about" 
            @click="closeMobileMenu"
            class="block py-2 md:py-3 px-3 md:px-4 text-gray-600 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 hover:bg-blue-50 dark:hover:bg-gray-700 transition-all duration-200 rounded-lg mx-2"
          >
            <div class="flex items-center space-x-3">
              <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path>
              </svg>
              <span>关于</span>
            </div>
          </NuxtLink>
          
          <div class="border-t border-gray-200 dark:border-gray-600 my-2 mx-2"></div>
          
          <!-- 移动端主题切换 -->
          <button 
            @click="toggleTheme"
            class="block w-full py-2 md:py-3 px-3 md:px-4 text-gray-600 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 hover:bg-blue-50 dark:hover:bg-gray-700 transition-all duration-200 rounded-lg mx-2 text-left"
          >
            <div class="flex items-center space-x-3">
              <svg v-if="isDark" class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 3v1m0 16v1m9-9h-1M4 12H3m15.364 6.364l-.707-.707M6.343 6.343l-.707-.707m12.728 0l-.707.707M6.343 17.657l-.707.707M16 12a4 4 0 11-8 0 4 4 0 018 0z"></path>
              </svg>
              <svg v-else class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M20.354 15.354A9 9 0 018.646 3.646 9.003 9.003 0 0012 21a9.003 9.003 0 008.354-5.646z"></path>
              </svg>
              <span>{{ isDark ? '浅色模式' : '深色模式' }}</span>
            </div>
          </button>
          
          <!-- 移动端语言切换（暂时隐藏） -->
          <!-- <button 
            @click="toggleLanguage"
            class="block w-full py-2 md:py-3 px-3 md:px-4 text-gray-600 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 hover:bg-blue-50 dark:hover:bg-gray-700 transition-all duration-200 rounded-lg mx-2 text-left"
          >
            <div class="flex items-center space-x-3">
              <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5h12M9 3v2m1.048 9.5A18.022 18.022 0 016.412 9m6.088 9h7M11 21l5-10 5 10M12.751 5C11.783 10.77 8.07 15.61 3 18.129"></path>
              </svg>
              <span>{{ isEnglish ? '中文' : 'English' }}</span>
            </div>
          </button> -->
          
          <!-- 移动端GitHub链接 -->
          <a 
            href="https://github.com/yourusername/nuxtnotion" 
            target="_blank" 
            rel="noopener noreferrer"
            @click="closeMobileMenu"
            class="block py-2 md:py-3 px-3 md:px-4 text-gray-600 dark:text-gray-300 hover:text-blue-600 dark:hover:text-blue-400 hover:bg-blue-50 dark:hover:bg-gray-700 transition-all duration-200 rounded-lg mx-2"
          >
            <div class="flex items-center space-x-3">
              <svg class="w-5 h-5" fill="currentColor" viewBox="0 0 24 24">
                <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
              </svg>
              <span>GitHub</span>
            </div>
          </a>
        </div>
      </div>
    </div>
  </nav>
</template>

<script setup>
const mobileMenuOpen = ref(false)

// 主题状态
const isDark = ref(false)

// 语言状态（暂时隐藏）
// const isEnglish = ref(false)

// 检查初始主题
onMounted(() => {
  // 检查localStorage中的主题设置
  const savedTheme = localStorage.getItem('theme')
  if (savedTheme) {
    isDark.value = savedTheme === 'dark'
  } else {
    // 检查系统主题偏好
    isDark.value = window.matchMedia('(prefers-color-scheme: dark)').matches
  }
  
  // 应用主题
  if (isDark.value) {
    document.documentElement.classList.add('dark')
  } else {
    document.documentElement.classList.remove('dark')
  }
})

// 切换移动端菜单
const toggleMobileMenu = () => {
  mobileMenuOpen.value = !mobileMenuOpen.value
}

// 关闭移动端菜单
const closeMobileMenu = () => {
  mobileMenuOpen.value = false
}

// 主题切换功能
const toggleTheme = () => {
  isDark.value = !isDark.value
  
  if (isDark.value) {
    document.documentElement.classList.add('dark')
    localStorage.setItem('theme', 'dark')
  } else {
    document.documentElement.classList.remove('dark')
    localStorage.setItem('theme', 'light')
  }
}

// 语言切换功能（暂时隐藏）
// const toggleLanguage = () => {
//   isEnglish.value = !isEnglish.value
//   // 这里可以添加实际的语言切换逻辑
// }

// 监听路由变化，关闭移动端菜单
watch(() => useRoute().path, () => {
  closeMobileMenu()
})
</script>