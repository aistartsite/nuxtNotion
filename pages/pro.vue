<template>
  <div class="min-h-screen bg-gradient-to-br from-gray-50 via-white to-blue-50 dark:from-gray-900 dark:via-gray-800 dark:to-blue-900">
    <!-- Hero Section -->
    <section class="relative overflow-hidden py-20 lg:py-32">
      <!-- 背景装饰 -->
      <div class="absolute inset-0">
        <div class="absolute top-0 left-0 w-72 h-72 bg-gradient-to-br from-blue-400/20 to-purple-600/20 rounded-full blur-3xl transform -translate-x-1/2 -translate-y-1/2"></div>
        <div class="absolute bottom-0 right-0 w-96 h-96 bg-gradient-to-br from-orange-400/20 to-pink-600/20 rounded-full blur-3xl transform translate-x-1/2 translate-y-1/2"></div>
      </div>
      
      <div class="container mx-auto px-4 relative z-10">
        <div class="text-center max-w-4xl mx-auto">
          <!-- PRO标识 -->
          <div class="inline-flex items-center space-x-2 bg-gradient-to-r from-orange-500 to-red-500 text-white px-4 py-2 rounded-full text-sm font-medium mb-6">
            <svg class="w-4 h-4" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6.253v13m0-13C10.832 5.477 9.246 5 7.5 5S4.168 5.477 3 6.253v13C4.168 18.477 5.754 18 7.5 18s3.332.477 4.5 1.253m0-13C13.168 5.477 14.754 5 16.5 5c1.747 0 3.332.477 4.5 1.253v13C19.832 18.477 18.247 18 16.5 18c-1.746 0-3.332.477-4.5 1.253"></path>
            </svg>
            <span>NuxtNotion PRO</span>
          </div>
          
          <h1 class="text-4xl md:text-6xl lg:text-7xl font-bold mb-6">
            <span class="bg-gradient-to-r from-orange-500 via-red-500 to-pink-500 bg-clip-text text-transparent">
              企业级知识付费平台
            </span>
          </h1>
          
          <p class="text-xl md:text-2xl text-gray-600 dark:text-gray-300 mb-8 leading-relaxed">
            专业的知识变现解决方案，助力企业构建完整的付费内容生态
          </p>
          
          <div class="flex flex-col sm:flex-row gap-4 justify-center items-center">
            <button class="group relative px-8 py-4 bg-gradient-to-r from-orange-500 to-red-500 text-white font-semibold rounded-xl shadow-lg hover:shadow-xl transform hover:-translate-y-1 transition-all duration-300">
              <span class="relative z-10">开启知识变现</span>
              <div class="absolute inset-0 bg-gradient-to-r from-orange-600 to-red-600 rounded-xl opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
            </button>
            <button @click="scrollToSection('success-cases')" class="px-8 py-4 border-2 border-gray-300 dark:border-gray-600 text-gray-700 dark:text-gray-300 font-semibold rounded-xl hover:border-orange-500 hover:text-orange-500 transition-all duration-300">
              查看案例
            </button>
          </div>
        </div>
      </div>
    </section>

    <!-- 核心功能对比 -->
    <section class="py-20 bg-white/50 dark:bg-gray-800/50 backdrop-blur-sm">
      <div class="container mx-auto px-4">
        <div class="text-center mb-16">
          <h2 class="text-3xl md:text-4xl font-bold text-gray-900 dark:text-white mb-4">
            基础版 vs 高级版
          </h2>
          <p class="text-xl text-gray-600 dark:text-gray-300">
            选择适合您的知识付费解决方案
          </p>
        </div>
        
        <div class="max-w-6xl mx-auto">
          <div class="grid md:grid-cols-3 gap-8">
            <!-- 基础版 -->
            <div class="bg-white dark:bg-gray-800 rounded-2xl p-8 shadow-lg border border-gray-200 dark:border-gray-700">
              <div class="text-center mb-8">
                <h3 class="text-2xl font-bold text-gray-900 dark:text-white mb-2">基础版</h3>
                <p class="text-gray-600 dark:text-gray-300">适合个人创作者</p>
                <div class="mt-4">
                  <div class="text-sm text-gray-500 dark:text-gray-400 line-through mb-1">原价 $19.9/月</div>
                  <span class="text-3xl font-bold text-gray-900 dark:text-white">$9.9</span>
                  <span class="text-gray-600 dark:text-gray-300">/月</span>
                </div>
              </div>
              
              <ul class="space-y-4">
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300">基础内容发布</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300">简单付费墙</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300">基础用户管理</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300">月度数据报告</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
                  </svg>
                  <span class="text-gray-400 line-through">高级会员体系</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
                  </svg>
                  <span class="text-gray-400 line-through">企业级部署</span>
                </li>
              </ul>
            </div>
            
            <!-- 专业版 -->
            <div class="bg-gradient-to-br from-blue-50 to-purple-50 dark:from-blue-900/20 dark:to-purple-900/20 rounded-2xl p-8 shadow-xl border-2 border-blue-200 dark:border-blue-800 relative">
              <div class="absolute -top-4 left-1/2 transform -translate-x-1/2">
                <span class="bg-gradient-to-r from-blue-500 to-purple-500 text-white px-4 py-2 rounded-full text-sm font-medium">
                  推荐
                </span>
              </div>
              
              <div class="text-center mb-8">
                <h3 class="text-2xl font-bold text-gray-900 dark:text-white mb-2">专业版</h3>
                <p class="text-gray-600 dark:text-gray-300">适合专业团队</p>
                <div class="mt-4">
                  <div class="text-sm text-gray-500 dark:text-gray-400 line-through mb-1">原价 $49.9/月</div>
                  <span class="text-3xl font-bold text-blue-600 dark:text-blue-400">$29.9</span>
                  <span class="text-gray-600 dark:text-gray-300">/月</span>
                </div>
              </div>
              
              <ul class="space-y-4">
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300">包含基础版功能</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-blue-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300 font-medium">多层级会员体系</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-blue-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300 font-medium">课程订阅功能</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-blue-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300 font-medium">营销工具套件</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-blue-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300 font-medium">实时数据分析</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
                  </svg>
                  <span class="text-gray-400 line-through">企业级部署</span>
                </li>
              </ul>
            </div>
            
            <!-- 企业版 -->
            <div class="bg-white dark:bg-gray-800 rounded-2xl p-8 shadow-lg border border-gray-200 dark:border-gray-700">
              <div class="text-center mb-8">
                <h3 class="text-2xl font-bold text-gray-900 dark:text-white mb-2">企业版</h3>
                <p class="text-gray-600 dark:text-gray-300">大型企业首选</p>
                <div class="mt-4">
                  <div class="text-sm text-gray-500 dark:text-gray-400 line-through mb-1">原价 $2999/年</div>
                  <span class="text-3xl font-bold text-gray-900 dark:text-white">$1999</span>
                  <span class="text-gray-600 dark:text-gray-300">/年</span>
                </div>
              </div>
              
              <ul class="space-y-4">
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300">包含专业版功能</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300 font-medium">企业级私有部署</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300 font-medium">定制化开发</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300 font-medium">专属客户经理</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300 font-medium">高级技术支持</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300 font-medium">SLA服务保障</span>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- 核心功能展示 -->
    <section class="py-20">
      <div class="container mx-auto px-4">
        <div class="text-center mb-16">
          <h2 class="text-3xl md:text-4xl font-bold text-gray-900 dark:text-white mb-4">
            知识付费核心功能
          </h2>
          <p class="text-xl text-gray-600 dark:text-gray-300">
            专为知识变现打造的完整解决方案
          </p>
        </div>
        
        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
          <!-- 付费解锁文章 -->
          <div class="group bg-white dark:bg-gray-800 rounded-2xl p-8 shadow-lg hover:shadow-xl transition-all duration-300 border border-gray-200 dark:border-gray-700 hover:border-orange-300 dark:hover:border-orange-600">
            <div class="w-12 h-12 bg-gradient-to-br from-blue-500 to-purple-600 rounded-xl flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
              <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 15v2m-6 4h12a2 2 0 002-2v-6a2 2 0 00-2-2H6a2 2 0 00-2 2v6a2 2 0 002 2zm10-10V7a4 4 0 00-8 0v4h8z"></path>
              </svg>
            </div>
            <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">付费解锁文章</h3>
            <p class="text-gray-600 dark:text-gray-300 mb-4">灵活的内容付费模式，支持单篇付费、打包销售等多种变现方式。</p>
            <ul class="text-sm text-gray-500 dark:text-gray-400 space-y-1">
              <li>• 单篇文章付费</li>
              <li>• 专栏打包销售</li>
              <li>• 免费试读设置</li>
              <li>• 动态定价策略</li>
            </ul>
          </div>
          
          <!-- 会员订阅系统 -->
          <div class="group bg-white dark:bg-gray-800 rounded-2xl p-8 shadow-lg hover:shadow-xl transition-all duration-300 border border-gray-200 dark:border-gray-700 hover:border-orange-300 dark:hover:border-orange-600">
            <div class="w-12 h-12 bg-gradient-to-br from-green-500 to-emerald-600 rounded-xl flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
              <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"></path>
              </svg>
            </div>
            <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">会员订阅系统</h3>
            <p class="text-gray-600 dark:text-gray-300 mb-4">多层级会员体系，提供持续稳定的订阅收入模式。</p>
            <ul class="text-sm text-gray-500 dark:text-gray-400 space-y-1">
              <li>• 多层级会员等级</li>
              <li>• 月度/年度订阅</li>
              <li>• 会员专属内容</li>
              <li>• 自动续费管理</li>
            </ul>
          </div>
          
          <!-- 课程体系 -->
          <div class="group bg-white dark:bg-gray-800 rounded-2xl p-8 shadow-lg hover:shadow-xl transition-all duration-300 border border-gray-200 dark:border-gray-700 hover:border-orange-300 dark:hover:border-orange-600">
            <div class="w-12 h-12 bg-gradient-to-br from-purple-500 to-pink-600 rounded-xl flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
              <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6.253v13m0-13C10.832 5.477 9.246 5 7.5 5S4.168 5.477 3 6.253v13C4.168 18.477 5.754 18 7.5 18s3.332.477 4.5 1.253m0-13C13.168 5.477 14.754 5 16.5 5c1.747 0 3.332.477 4.5 1.253v13C19.832 18.477 18.247 18 16.5 18c-1.746 0-3.332.477-4.5 1.253"></path>
              </svg>
            </div>
            <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">在线课程体系</h3>
            <p class="text-gray-600 dark:text-gray-300 mb-4">完整的在线教育解决方案，支持视频课程、直播教学等多种形式。</p>
            <ul class="text-sm text-gray-500 dark:text-gray-400 space-y-1">
              <li>• 视频课程管理</li>
              <li>• 直播教学功能</li>
              <li>• 学习进度跟踪</li>
              <li>• 作业与考试系统</li>
            </ul>
          </div>
          
          <!-- 营销工具 -->
          <div class="group bg-white dark:bg-gray-800 rounded-2xl p-8 shadow-lg hover:shadow-xl transition-all duration-300 border border-gray-200 dark:border-gray-700 hover:border-orange-300 dark:hover:border-orange-600">
            <div class="w-12 h-12 bg-gradient-to-br from-yellow-500 to-orange-600 rounded-xl flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
              <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M11 5.882V19.24a1.76 1.76 0 01-3.417.592l-2.147-6.15M18 13a3 3 0 100-6M5.436 13.683A4.001 4.001 0 017 6h1.832c4.1 0 7.625-1.234 9.168-3v14c-1.543-1.766-5.067-3-9.168-3H7a3.988 3.988 0 01-1.564-.317z"></path>
              </svg>
            </div>
            <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">智能营销工具</h3>
            <p class="text-gray-600 dark:text-gray-300 mb-4">强大的营销推广工具，帮助您快速获取用户和提升转化率。</p>
            <ul class="text-sm text-gray-500 dark:text-gray-400 space-y-1">
              <li>• 优惠券系统</li>
              <li>• 分销推广</li>
              <li>• 邀请返利</li>
              <li>• 限时促销活动</li>
            </ul>
          </div>
          
          <!-- 数据分析 -->
          <div class="group bg-white dark:bg-gray-800 rounded-2xl p-8 shadow-lg hover:shadow-xl transition-all duration-300 border border-gray-200 dark:border-gray-700 hover:border-orange-300 dark:hover:border-orange-600">
            <div class="w-12 h-12 bg-gradient-to-br from-indigo-500 to-blue-600 rounded-xl flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
              <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z"></path>
              </svg>
            </div>
            <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">数据分析中心</h3>
            <p class="text-gray-600 dark:text-gray-300 mb-4">全方位的数据分析和用户洞察，助您优化运营策略。</p>
            <ul class="text-sm text-gray-500 dark:text-gray-400 space-y-1">
              <li>• 收入数据分析</li>
              <li>• 用户行为追踪</li>
              <li>• 内容表现统计</li>
              <li>• 转化漏斗分析</li>
            </ul>
          </div>
          
          <!-- 企业级部署 -->
          <div class="group bg-white dark:bg-gray-800 rounded-2xl p-8 shadow-lg hover:shadow-xl transition-all duration-300 border border-gray-200 dark:border-gray-700 hover:border-orange-300 dark:hover:border-orange-600">
            <div class="w-12 h-12 bg-gradient-to-br from-red-500 to-pink-600 rounded-xl flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
              <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 12h14M5 12a2 2 0 01-2-2V6a2 2 0 012-2h14a2 2 0 012 2v4a2 2 0 01-2 2M5 12a2 2 0 00-2 2v4a2 2 0 002 2h14a2 2 0 002-2v-4a2 2 0 00-2-2m-2-4h.01M17 16h.01"></path>
              </svg>
            </div>
            <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">企业级部署</h3>
            <p class="text-gray-600 dark:text-gray-300 mb-4">专业的私有化部署方案，确保数据安全和系统稳定性。</p>
            <ul class="text-sm text-gray-500 dark:text-gray-400 space-y-1">
              <li>• 私有云部署</li>
              <li>• 数据安全保障</li>
              <li>• 定制化开发</li>
              <li>• 专属技术支持</li>
            </ul>
          </div>
        </div>
      </div>
    </section>

    <!-- 使用案例 -->
    <section class="py-20 bg-white/50 dark:bg-gray-800/50 backdrop-blur-sm">
      <div class="container mx-auto px-4">
        <div class="text-center mb-16">
          <h2 class="text-3xl md:text-4xl font-bold text-gray-900 dark:text-white mb-4">
            适用场景
          </h2>
          <p class="text-xl text-gray-600 dark:text-gray-300">
            NuxtNotion PRO 适合各种商业应用场景
          </p>
        </div>
        
        <div class="grid md:grid-cols-2 lg:grid-cols-4 gap-8">
          <div class="text-center group">
            <div class="w-16 h-16 bg-gradient-to-br from-blue-500 to-purple-600 rounded-2xl flex items-center justify-center mx-auto mb-4 group-hover:scale-110 transition-transform duration-300">
              <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 14l9-5-9-5-9 5 9 5z"></path>
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 14l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14z"></path>
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 14l9-5-9-5-9 5 9 5zm0 0l6.16-3.422a12.083 12.083 0 01.665 6.479A11.952 11.952 0 0012 20.055a11.952 11.952 0 00-6.824-2.998 12.078 12.078 0 01.665-6.479L12 14zm-4 6v-7.5l4-2.222"></path>
              </svg>
            </div>
            <h3 class="text-lg font-bold text-gray-900 dark:text-white mb-2">在线教育</h3>
            <p class="text-gray-600 dark:text-gray-300 text-sm">K12教育、职业培训、技能认证</p>
          </div>
          
          <div class="text-center group">
            <div class="w-16 h-16 bg-gradient-to-br from-green-500 to-emerald-600 rounded-2xl flex items-center justify-center mx-auto mb-4 group-hover:scale-110 transition-transform duration-300">
              <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 21V5a2 2 0 00-2-2H7a2 2 0 00-2 2v16m14 0h2m-2 0h-4m-5 0H9m0 0H5m0 0h2M7 7h10M7 11h10M7 15h10"></path>
              </svg>
            </div>
            <h3 class="text-lg font-bold text-gray-900 dark:text-white mb-2">企业管理</h3>
            <p class="text-gray-600 dark:text-gray-300 text-sm">管理培训、领导力发展、团队建设</p>
          </div>
          
          <div class="text-center group">
            <div class="w-16 h-16 bg-gradient-to-br from-purple-500 to-pink-600 rounded-2xl flex items-center justify-center mx-auto mb-4 group-hover:scale-110 transition-transform duration-300">
              <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.663 17h4.673M12 3v1m6.364 1.636l-.707.707M21 12h-1M4 12H3m3.343-5.657l-.707-.707m2.828 9.9a5 5 0 117.072 0l-.548.547A3.374 3.374 0 0014 18.469V19a2 2 0 11-4 0v-.531c0-.895-.356-1.754-.988-2.386l-.548-.547z"></path>
              </svg>
            </div>
            <h3 class="text-lg font-bold text-gray-900 dark:text-white mb-2">专业咨询</h3>
            <p class="text-gray-600 dark:text-gray-300 text-sm">法律咨询、财务顾问、医疗健康</p>
          </div>
          
          <div class="text-center group">
            <div class="w-16 h-16 bg-gradient-to-br from-orange-500 to-red-600 rounded-2xl flex items-center justify-center mx-auto mb-4 group-hover:scale-110 transition-transform duration-300">
              <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0zm6 3a2 2 0 11-4 0 2 2 0 014 0zM7 10a2 2 0 11-4 0 2 2 0 014 0z"></path>
              </svg>
            </div>
            <h3 class="text-lg font-bold text-gray-900 dark:text-white mb-2">社区平台</h3>
            <p class="text-gray-600 dark:text-gray-300 text-sm">用户社区，论坛，会员交流等社交功能</p>
          </div>
        </div>
      </div>
    </section>

    <!-- 成功案例 -->
    <section id="success-cases" class="py-20 bg-gray-50 dark:bg-gray-900">
      <div class="container mx-auto px-4">
        <div class="text-center mb-16">
          <h2 class="text-3xl md:text-4xl font-bold text-gray-900 dark:text-white mb-4">
            成功案例
          </h2>
          <p class="text-xl text-gray-600 dark:text-gray-300">
            看看他们如何通过知识付费实现财富自由
          </p>
        </div>
        
        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
          <div class="bg-white dark:bg-gray-800 rounded-2xl p-8 shadow-lg">
            <div class="flex items-center mb-6">
              <img src="https://images.unsplash.com/photo-1472099645785-5658abf4ff4e?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="客户头像" class="w-12 h-12 rounded-full mr-4">
              <div>
                <h4 class="font-bold text-gray-900 dark:text-white">陈老师</h4>
                <p class="text-gray-600 dark:text-gray-300 text-sm">编程教育专家</p>
              </div>
            </div>
            <p class="text-gray-600 dark:text-gray-300 mb-4">
              "通过平台发布编程课程，6个月内获得了50万+学员，月收入突破100万元。"
            </p>
            <div class="flex items-center justify-between text-sm text-gray-500 dark:text-gray-400">
              <span>月收入: ¥1,000,000+</span>
              <span>学员数: 50万+</span>
            </div>
            <div class="mt-4 bg-gradient-to-r from-green-500 to-emerald-600 h-2 rounded-full"></div>
          </div>
          
          <div class="bg-white dark:bg-gray-800 rounded-2xl p-8 shadow-lg">
            <div class="flex items-center mb-6">
              <img src="https://api.dicebear.com/7.x/avataaars/svg?seed=lisa&backgroundColor=b6e3f4,c0aede,d1d4f9" alt="客户头像" class="w-12 h-12 rounded-full mr-4">
              <div>
                <h4 class="font-bold text-gray-900 dark:text-white">李博士</h4>
                <p class="text-gray-600 dark:text-gray-300 text-sm">金融分析师</p>
              </div>
            </div>
            <p class="text-gray-600 dark:text-gray-300 mb-4">
              "专注投资理财内容创作，付费订阅用户达到20万，实现了知识变现的梦想。"
            </p>
            <div class="flex items-center justify-between text-sm text-gray-500 dark:text-gray-400">
              <span>月收入: ¥500,000+</span>
              <span>订阅用户: 20万+</span>
            </div>
            <div class="mt-4 bg-gradient-to-r from-blue-500 to-purple-600 h-2 rounded-full"></div>
          </div>
          
          <div class="bg-white dark:bg-gray-800 rounded-2xl p-8 shadow-lg">
            <div class="flex items-center mb-6">
              <img src="https://images.unsplash.com/photo-1519244703995-f4e0f30006d5?ixlib=rb-1.2.1&ixid=eyJhcHBfaWQiOjEyMDd9&auto=format&fit=facearea&facepad=2&w=256&h=256&q=80" alt="客户头像" class="w-12 h-12 rounded-full mr-4">
              <div>
                <h4 class="font-bold text-gray-900 dark:text-white">王总</h4>
                <p class="text-gray-600 dark:text-gray-300 text-sm">企业管理顾问</p>
              </div>
            </div>
            <p class="text-gray-600 dark:text-gray-300 mb-4">
              "为企业提供管理培训课程，企业版客户续费率达95%，年收入超过800万。"
            </p>
            <div class="flex items-center justify-between text-sm text-gray-500 dark:text-gray-400">
              <span>年收入: ¥8,000,000+</span>
              <span>续费率: 95%</span>
            </div>
            <div class="mt-4 bg-gradient-to-r from-yellow-500 to-orange-600 h-2 rounded-full"></div>
          </div>
        </div>
        
        <!-- 数据统计 -->
        <div class="mt-16 grid md:grid-cols-4 gap-8 text-center">
          <div class="bg-white dark:bg-gray-800 rounded-2xl p-6 shadow-lg">
            <div class="text-3xl font-bold text-orange-600 mb-2">10,000+</div>
            <div class="text-gray-600 dark:text-gray-300">内容创作者</div>
          </div>
          <div class="bg-white dark:bg-gray-800 rounded-2xl p-6 shadow-lg">
            <div class="text-3xl font-bold text-blue-600 mb-2">50万+</div>
            <div class="text-gray-600 dark:text-gray-300">付费用户</div>
          </div>
          <div class="bg-white dark:bg-gray-800 rounded-2xl p-6 shadow-lg">
            <div class="text-3xl font-bold text-green-600 mb-2">50亿+</div>
            <div class="text-gray-600 dark:text-gray-300">累计交易额</div>
          </div>
          <div class="bg-white dark:bg-gray-800 rounded-2xl p-6 shadow-lg">
            <div class="text-3xl font-bold text-purple-600 mb-2">98%</div>
            <div class="text-gray-600 dark:text-gray-300">用户满意度</div>
          </div>
        </div>
      </div>
    </section>

    <!-- FAQ Section -->
    <section class="py-20">
      <div class="container mx-auto px-4">
        <div class="text-center mb-16">
          <h2 class="text-3xl md:text-4xl font-bold text-gray-900 dark:text-white mb-4">
            常见问题
          </h2>
          <p class="text-xl text-gray-600 dark:text-gray-300">
            解答您关于知识付费平台的疑问
          </p>
        </div>
        
        <div class="max-w-4xl mx-auto">
          <div class="space-y-6">
            <div class="bg-white dark:bg-gray-800 rounded-2xl p-6 shadow-lg border border-gray-200 dark:border-gray-700">
              <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">如何开始创建付费内容？</h3>
              <p class="text-gray-600 dark:text-gray-300">注册账号后，您可以立即开始创建内容。平台提供丰富的编辑工具，支持文章、视频、音频等多种形式。您可以设置免费试读部分，然后为完整内容设定价格。我们的智能推荐系统会帮助您的内容触达更多潜在用户。</p>
            </div>
            
            <div class="bg-white dark:bg-gray-800 rounded-2xl p-6 shadow-lg border border-gray-200 dark:border-gray-700">
              <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">支持哪些支付方式？</h3>
              <p class="text-gray-600 dark:text-gray-300">平台支持微信支付、支付宝、银行卡、PayPal等多种支付方式。企业版还支持对公转账、发票开具等企业级支付需求。所有交易都经过银行级加密保护，确保资金安全。</p>
            </div>
            
            <div class="bg-white dark:bg-gray-800 rounded-2xl p-6 shadow-lg border border-gray-200 dark:border-gray-700">
              <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">如何保护我的知识产权？</h3>
              <p class="text-gray-600 dark:text-gray-300">我们采用多重版权保护机制：内容加密传输、防盗链技术、水印保护、访问权限控制等。同时提供法律维权支持，一旦发现侵权行为，我们会协助您进行维权。企业版还提供专属的知识产权保护服务。</p>
            </div>
            
            <div class="bg-white dark:bg-gray-800 rounded-2xl p-6 shadow-lg border border-gray-200 dark:border-gray-700">
              <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">可以自定义品牌和域名吗？</h3>
              <p class="text-gray-600 dark:text-gray-300">专业版和企业版支持自定义品牌LOGO、色彩主题和页面布局。企业版还支持独立域名绑定，让您拥有完全独立的品牌形象。我们提供专业的UI/UX设计服务，帮助您打造独特的品牌体验。</p>
            </div>
            
            <div class="bg-white dark:bg-gray-800 rounded-2xl p-6 shadow-lg border border-gray-200 dark:border-gray-700">
              <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">提供哪些数据分析功能？</h3>
              <p class="text-gray-600 dark:text-gray-300">平台提供全面的数据分析：用户行为分析、内容表现统计、收入趋势分析、转化漏斗分析等。企业版还包含高级分析功能如用户画像、A/B测试、预测分析等，帮助您优化内容策略和提升转化率。</p>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- CTA Section -->
    <section class="py-20 relative overflow-hidden">
      <div class="absolute inset-0 bg-gradient-to-br from-orange-600 via-red-600 to-purple-700"></div>
      <div class="absolute inset-0 bg-black opacity-50"></div>
      <div class="container mx-auto px-4 relative z-10">
        <div class="text-center">
          <h2 class="text-3xl md:text-5xl font-bold text-white mb-6">
            准备开始您的企业级知识付费之旅？
          </h2>
          <p class="text-xl text-gray-200 mb-8 max-w-3xl mx-auto">
            立即升级到PRO版，解锁所有高级功能，让您的知识变现之路更加顺畅
          </p>
          <div class="flex flex-col sm:flex-row gap-4 justify-center">
            <button class="bg-white text-gray-900 px-8 py-4 rounded-xl font-bold text-lg hover:bg-gray-100 transition-colors duration-300 shadow-lg">
              立即升级PRO版
            </button>
            <button class="border-2 border-white text-white px-8 py-4 rounded-xl font-bold text-lg hover:bg-white hover:text-gray-900 transition-colors duration-300">
              预约演示
            </button>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script setup>
// 页面元数据
useHead({
  title: 'NuxtNotion PRO - 企业级 Notion 建站解决方案',
  meta: [
    {
      name: 'description',
      content: 'NuxtNotion PRO版提供企业级功能，包括高级组件库、电商系统、会员管理、支付集成等，助您构建专业的商业网站。'
    },
    {
      property: 'og:title',
      content: 'NuxtNotion PRO - 企业级 Notion 建站解决方案'
    },
    {
      property: 'og:description',
      content: 'NuxtNotion PRO版提供企业级功能，包括高级组件库、电商系统、会员管理、支付集成等，助您构建专业的商业网站。'
    },
    {
      property: 'og:type',
      content: 'website'
    }
  ]
})

// 滚动到指定部分
const scrollToSection = (sectionId) => {
  const element = document.getElementById(sectionId)
  if (element) {
    element.scrollIntoView({ 
      behavior: 'smooth',
      block: 'start'
    })
  }
}
</script>