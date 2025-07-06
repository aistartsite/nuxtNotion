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
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 3v4M3 5h4M6 17v4m-2-2h4m5-16l2.286 6.857L21 12l-5.714 2.143L13 21l-2.286-6.857L5 12l5.714-2.143L13 3z"></path>
            </svg>
            <span>NuxtNotion PRO</span>
          </div>
          
          <h1 class="text-4xl md:text-6xl lg:text-7xl font-bold mb-6">
            <span class="bg-gradient-to-r from-orange-500 via-red-500 to-pink-500 bg-clip-text text-transparent">
              企业级建站解决方案
            </span>
          </h1>
          
          <p class="text-xl md:text-2xl text-gray-600 dark:text-gray-300 mb-8 leading-relaxed">
            专为企业和专业团队设计的高级功能，助您构建完整的商业网站
          </p>
          
          <div class="flex flex-col sm:flex-row gap-4 justify-center items-center">
            <button class="group relative px-8 py-4 bg-gradient-to-r from-orange-500 to-red-500 text-white font-semibold rounded-xl shadow-lg hover:shadow-xl transform hover:-translate-y-1 transition-all duration-300">
              <span class="relative z-10">立即升级 PRO</span>
              <div class="absolute inset-0 bg-gradient-to-r from-orange-600 to-red-600 rounded-xl opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
            </button>
            <button class="px-8 py-4 border-2 border-gray-300 dark:border-gray-600 text-gray-700 dark:text-gray-300 font-semibold rounded-xl hover:border-orange-500 hover:text-orange-500 transition-all duration-300">
              查看演示
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
            免费版 vs PRO版
          </h2>
          <p class="text-xl text-gray-600 dark:text-gray-300">
            解锁更多强大功能，满足企业级需求
          </p>
        </div>
        
        <div class="max-w-6xl mx-auto">
          <div class="grid md:grid-cols-2 gap-8">
            <!-- 免费版 -->
            <div class="bg-white dark:bg-gray-800 rounded-2xl p-8 shadow-lg border border-gray-200 dark:border-gray-700">
              <div class="text-center mb-8">
                <h3 class="text-2xl font-bold text-gray-900 dark:text-white mb-2">免费版</h3>
                <p class="text-gray-600 dark:text-gray-300">适合个人博客和小型项目</p>
                <div class="mt-4">
                  <span class="text-3xl font-bold text-gray-900 dark:text-white">¥0</span>
                  <span class="text-gray-600 dark:text-gray-300">/月</span>
                </div>
              </div>
              
              <ul class="space-y-4">
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300">基础博客功能</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300">响应式设计</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300">SEO 优化</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300">基础主题</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
                  </svg>
                  <span class="text-gray-400 line-through">高级组件库</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
                  </svg>
                  <span class="text-gray-400 line-through">电商功能</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12"></path>
                  </svg>
                  <span class="text-gray-400 line-through">会员系统</span>
                </li>
              </ul>
            </div>
            
            <!-- PRO版 -->
            <div class="bg-gradient-to-br from-orange-50 to-red-50 dark:from-orange-900/20 dark:to-red-900/20 rounded-2xl p-8 shadow-xl border-2 border-orange-200 dark:border-orange-800 relative">
              <div class="absolute -top-4 left-1/2 transform -translate-x-1/2">
                <span class="bg-gradient-to-r from-orange-500 to-red-500 text-white px-4 py-2 rounded-full text-sm font-medium">
                  推荐
                </span>
              </div>
              
              <div class="text-center mb-8">
                <h3 class="text-2xl font-bold text-gray-900 dark:text-white mb-2">PRO版</h3>
                <p class="text-gray-600 dark:text-gray-300">企业级功能，商业网站首选</p>
                <div class="mt-4">
                  <span class="text-3xl font-bold text-orange-600 dark:text-orange-400">$1999</span>
                  <span class="text-gray-600 dark:text-gray-300">/年</span>
                </div>
              </div>
              
              <ul class="space-y-4">
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-green-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300">包含所有免费功能</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-orange-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300 font-medium">50+ 高级组件</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-orange-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300 font-medium">电商购物车系统</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-orange-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300 font-medium">用户会员系统</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-orange-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300 font-medium">支付集成</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-orange-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300 font-medium">数据分析面板</span>
                </li>
                <li class="flex items-center space-x-3">
                  <svg class="w-5 h-5 text-orange-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"></path>
                  </svg>
                  <span class="text-gray-700 dark:text-gray-300 font-medium">优先技术支持</span>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </section>

    <!-- PRO功能展示 -->
    <section class="py-20">
      <div class="container mx-auto px-4">
        <div class="text-center mb-16">
          <h2 class="text-3xl md:text-4xl font-bold text-gray-900 dark:text-white mb-4">
            PRO版独有功能
          </h2>
          <p class="text-xl text-gray-600 dark:text-gray-300">
            专为企业级应用设计的强大功能
          </p>
        </div>
        
        <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
          <!-- 高级组件库 -->
          <div class="group bg-white dark:bg-gray-800 rounded-2xl p-8 shadow-lg hover:shadow-xl transition-all duration-300 border border-gray-200 dark:border-gray-700 hover:border-orange-300 dark:hover:border-orange-600">
            <div class="w-12 h-12 bg-gradient-to-br from-blue-500 to-purple-600 rounded-xl flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
              <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10"></path>
              </svg>
            </div>
            <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">高级组件库</h3>
            <p class="text-gray-600 dark:text-gray-300 mb-4">50+ 精美组件，包括数据表格、图表、表单、模态框等企业级组件。</p>
            <ul class="text-sm text-gray-500 dark:text-gray-400 space-y-1">
              <li>• 数据表格与分页</li>
              <li>• 交互式图表</li>
              <li>• 高级表单组件</li>
              <li>• 文件上传组件</li>
            </ul>
          </div>
          
          <!-- 电商系统 -->
          <div class="group bg-white dark:bg-gray-800 rounded-2xl p-8 shadow-lg hover:shadow-xl transition-all duration-300 border border-gray-200 dark:border-gray-700 hover:border-orange-300 dark:hover:border-orange-600">
            <div class="w-12 h-12 bg-gradient-to-br from-green-500 to-emerald-600 rounded-xl flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
              <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 3h2l.4 2M7 13h10l4-8H5.4m0 0L7 13m0 0l-2.293 2.293c-.63.63-.184 1.707.707 1.707H17M17 13v6a2 2 0 01-2 2H9a2 2 0 01-2-2v-6m8 0V9a2 2 0 00-2-2H9a2 2 0 00-2 2v4.01"></path>
              </svg>
            </div>
            <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">电商购物系统</h3>
            <p class="text-gray-600 dark:text-gray-300 mb-4">完整的在线商店功能，支持产品管理、购物车、订单处理等。</p>
            <ul class="text-sm text-gray-500 dark:text-gray-400 space-y-1">
              <li>• 产品展示与管理</li>
              <li>• 购物车功能</li>
              <li>• 订单管理系统</li>
              <li>• 库存管理</li>
            </ul>
          </div>
          
          <!-- 会员系统 -->
          <div class="group bg-white dark:bg-gray-800 rounded-2xl p-8 shadow-lg hover:shadow-xl transition-all duration-300 border border-gray-200 dark:border-gray-700 hover:border-orange-300 dark:hover:border-orange-600">
            <div class="w-12 h-12 bg-gradient-to-br from-purple-500 to-pink-600 rounded-xl flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
              <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 4.354a4 4 0 110 5.292M15 21H3v-1a6 6 0 0112 0v1zm0 0h6v-1a6 6 0 00-9-5.197m13.5-9a2.5 2.5 0 11-5 0 2.5 2.5 0 015 0z"></path>
              </svg>
            </div>
            <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">用户会员系统</h3>
            <p class="text-gray-600 dark:text-gray-300 mb-4">完善的用户注册、登录、权限管理和会员等级系统。</p>
            <ul class="text-sm text-gray-500 dark:text-gray-400 space-y-1">
              <li>• 用户注册登录</li>
              <li>• 权限角色管理</li>
              <li>• 会员等级系统</li>
              <li>• 个人资料管理</li>
            </ul>
          </div>
          
          <!-- 支付集成 -->
          <div class="group bg-white dark:bg-gray-800 rounded-2xl p-8 shadow-lg hover:shadow-xl transition-all duration-300 border border-gray-200 dark:border-gray-700 hover:border-orange-300 dark:hover:border-orange-600">
            <div class="w-12 h-12 bg-gradient-to-br from-yellow-500 to-orange-600 rounded-xl flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
              <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 9V7a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2m2 4h10a2 2 0 002-2v-6a2 2 0 00-2-2H9a2 2 0 00-2 2v6a2 2 0 002 2zm7-5a2 2 0 11-4 0 2 2 0 014 0z"></path>
              </svg>
            </div>
            <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">支付集成</h3>
            <p class="text-gray-600 dark:text-gray-300 mb-4">集成主流支付平台，支持微信支付、支付宝、银行卡等多种支付方式。</p>
            <ul class="text-sm text-gray-500 dark:text-gray-400 space-y-1">
              <li>• 微信支付</li>
              <li>• 支付宝</li>
              <li>• 银行卡支付</li>
              <li>• 国际支付</li>
            </ul>
          </div>
          
          <!-- 数据分析 -->
          <div class="group bg-white dark:bg-gray-800 rounded-2xl p-8 shadow-lg hover:shadow-xl transition-all duration-300 border border-gray-200 dark:border-gray-700 hover:border-orange-300 dark:hover:border-orange-600">
            <div class="w-12 h-12 bg-gradient-to-br from-indigo-500 to-blue-600 rounded-xl flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
              <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 19v-6a2 2 0 00-2-2H5a2 2 0 00-2 2v6a2 2 0 002 2h2a2 2 0 002-2zm0 0V9a2 2 0 012-2h2a2 2 0 012 2v10m-6 0a2 2 0 002 2h2a2 2 0 002-2m0 0V5a2 2 0 012-2h2a2 2 0 012 2v14a2 2 0 01-2 2h-2a2 2 0 01-2-2z"></path>
              </svg>
            </div>
            <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">数据分析面板</h3>
            <p class="text-gray-600 dark:text-gray-300 mb-4">实时数据统计和分析，帮助您了解网站运营情况和用户行为。</p>
            <ul class="text-sm text-gray-500 dark:text-gray-400 space-y-1">
              <li>• 访问统计</li>
              <li>• 用户行为分析</li>
              <li>• 销售数据报表</li>
              <li>• 自定义仪表板</li>
            </ul>
          </div>
          
          <!-- 技术支持 -->
          <div class="group bg-white dark:bg-gray-800 rounded-2xl p-8 shadow-lg hover:shadow-xl transition-all duration-300 border border-gray-200 dark:border-gray-700 hover:border-orange-300 dark:hover:border-orange-600">
            <div class="w-12 h-12 bg-gradient-to-br from-red-500 to-pink-600 rounded-xl flex items-center justify-center mb-6 group-hover:scale-110 transition-transform duration-300">
              <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M18.364 5.636l-3.536 3.536m0 5.656l3.536 3.536M9.172 9.172L5.636 5.636m3.536 9.192L5.636 18.364M21 12a9 9 0 11-18 0 9 9 0 0118 0zm-5 0a4 4 0 11-8 0 4 4 0 018 0z"></path>
              </svg>
            </div>
            <h3 class="text-xl font-bold text-gray-900 dark:text-white mb-3">优先技术支持</h3>
            <p class="text-gray-600 dark:text-gray-300 mb-4">专业技术团队提供优先支持，确保您的项目顺利运行。</p>
            <ul class="text-sm text-gray-500 dark:text-gray-400 space-y-1">
              <li>• 专业技术支持</li>
              <li>• 专属部署服务</li>
              <li>• 定制方案</li>
              <li>• 长期维护和更新</li>
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
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 21V5a2 2 0 00-2-2H7a2 2 0 00-2 2v16m14 0h2m-2 0h-5m-9 0H3m2 0h5M9 7h1m-1 4h1m4-4h1m-1 4h1m-5 10v-5a1 1 0 011-1h2a1 1 0 011 1v5m-4 0h4"></path>
              </svg>
            </div>
            <h3 class="text-lg font-bold text-gray-900 dark:text-white mb-2">企业官网</h3>
            <p class="text-gray-600 dark:text-gray-300 text-sm">专业的企业形象展示，产品介绍，联系方式等</p>
          </div>
          
          <div class="text-center group">
            <div class="w-16 h-16 bg-gradient-to-br from-green-500 to-emerald-600 rounded-2xl flex items-center justify-center mx-auto mb-4 group-hover:scale-110 transition-transform duration-300">
              <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 11V7a4 4 0 00-8 0v4M5 9h14l1 12H4L5 9z"></path>
              </svg>
            </div>
            <h3 class="text-lg font-bold text-gray-900 dark:text-white mb-2">在线商城</h3>
            <p class="text-gray-600 dark:text-gray-300 text-sm">完整的电商功能，产品展示，购物车，支付系统</p>
          </div>
          
          <div class="text-center group">
            <div class="w-16 h-16 bg-gradient-to-br from-purple-500 to-pink-600 rounded-2xl flex items-center justify-center mx-auto mb-4 group-hover:scale-110 transition-transform duration-300">
              <svg class="w-8 h-8 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 6.253v13m0-13C10.832 5.477 9.246 5 7.5 5S4.168 5.477 3 6.253v13C4.168 18.477 5.754 18 7.5 18s3.332.477 4.5 1.253m0-13C13.168 5.477 14.754 5 16.5 5c1.747 0 3.332.477 4.5 1.253v13C19.832 18.477 18.247 18 16.5 18c-1.746 0-3.332.477-4.5 1.253"></path>
              </svg>
            </div>
            <h3 class="text-lg font-bold text-gray-900 dark:text-white mb-2">知识付费</h3>
            <p class="text-gray-600 dark:text-gray-300 text-sm">在线课程，会员内容，付费文章等知识变现</p>
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

    <!-- CTA Section -->
    <section class="py-20 relative overflow-hidden">
      <!-- 背景装饰 -->
      <div class="absolute inset-0">
        <div class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 w-96 h-96 bg-gradient-to-br from-orange-400/30 to-red-600/30 rounded-full blur-3xl"></div>
      </div>
      
      <div class="container mx-auto px-4 relative z-10">
        <div class="text-center max-w-3xl mx-auto">
          <h2 class="text-3xl md:text-4xl font-bold text-gray-900 dark:text-white mb-6">
            准备好升级到 PRO 版了吗？
          </h2>
          <p class="text-xl text-gray-600 dark:text-gray-300 mb-8">
            立即升级，解锁所有企业级功能，让您的网站更加专业和强大
          </p>
          
          <div class="flex flex-col sm:flex-row gap-4 justify-center items-center">
            <button class="group relative px-8 py-4 bg-gradient-to-r from-orange-500 to-red-500 text-white font-semibold rounded-xl shadow-lg hover:shadow-xl transform hover:-translate-y-1 transition-all duration-300">
              <span class="relative z-10 flex items-center space-x-2">
                <span>立即升级 PRO</span>
                <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 7l5 5m0 0l-5 5m5-5H6"></path>
                </svg>
              </span>
              <div class="absolute inset-0 bg-gradient-to-r from-orange-600 to-red-600 rounded-xl opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
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
</script>