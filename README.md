<html lang="zh-CN" class="scroll-smooth">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>IYKYK TICKET | 韩国本土预售票务管家 · Korean Presale Concierge</title>
<!-- Tailwind CSS -->
<script src="https://cdn.tailwindcss.com"></script>
<!-- Google Fonts -->
<link rel="preconnect" href="https://fonts.googleapis.com">
<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
<link href="https://fonts.googleapis.com/css2?family=Inter:wght@300;400;500;600;700;800&family=Noto+Sans+KR:wght@300;400;500;700&display=swap" rel="stylesheet">
<!-- Lucide Icons -->
<script src="https://unpkg.com/lucide@latest"></script>
<script>
tailwind.config = {
theme: {
extend: {
colors: {
kpink: {
50: '#FFF5F7',
100: '#FFE3E8',
200: '#FFD6E0',
300: '#FFB3C6',
400: '#FF85A1',
500: '#FF5C8A',
600: '#E03A6E',
700: '#C72557'
},
ktext: {
primary: '#2D3748',
secondary: '#718096',
light: '#A0AEC0'
},
kbg: '#FCF8F9'
},
fontFamily: {
sans: ['Inter', 'Noto Sans KR', 'sans-serif'],
},
borderRadius: {
'3xl': '1.75rem',
'4xl': '2.25rem',
'5xl': '2.75rem'
},
boxShadow: {
'soft': '0 12px 32px -8px rgba(255, 179, 198, 0.3)',
'soft-lg': '0 20px 48px -12px rgba(255, 133, 161, 0.35)',
'card': '0 8px 30px -6px rgba(113, 128, 150, 0.08)'
}
}
}
}
</script>
<style>
body {
background-color: #FCF8F9;
color: #2D3748;
font-family: 'Inter', 'Noto Sans KR', sans-serif;
overflow-x: hidden;
}
@keyframes floatSlow {
0%, 100% { transform: translateY(0px) rotate(0deg); }
50% { transform: translateY(-6px) rotate(1deg); }
}
@keyframes pulseGlow {
0%, 100% { opacity: 0.35; transform: scale(1); }
50% { opacity: 0.6; transform: scale(1.05); }
}
.animate-float-slow {
animation: floatSlow 6s ease-in-out infinite;
}
.animate-glow {
animation: pulseGlow 7s ease-in-out infinite;
}
.k-glass {
background: rgba(255, 255, 255, 0.92);
backdrop-filter: blur(16px);
-webkit-backdrop-filter: blur(16px);
border: 1px solid rgba(255, 214, 224, 0.7);
}
.no-scrollbar::-webkit-scrollbar {
display: none;
}
.no-scrollbar {
-ms-overflow-style: none;
scrollbar-width: none;
}
</style>
</head>
<body class="min-h-screen flex flex-col relative selection:bg-kpink-200 selection:text-kpink-600">
<!-- SUBTLE BACKGROUND DECORATIONS -->
<div class="absolute inset-0 pointer-events-none z-0 overflow-hidden">
<div class="absolute -top-24 -left-20 w-[32rem] h-[32rem] bg-kpink-100/70 rounded-full blur-3xl opacity-70 animate-glow"></div>
<div class="absolute top-1/3 -right-24 w-[28rem] h-[28rem] bg-kpink-200/50 rounded-full blur-3xl opacity-50 animate-glow" style="animation-delay: 2.5s;"></div>
<div class="absolute bottom-1/4 left-1/6 w-[30rem] h-[30rem] bg-rose-100/60 rounded-full blur-3xl opacity-60 animate-glow" style="animation-delay: 4.5s;"></div>
<div class="absolute inset-0 opacity-[0.02]" style="background-image: radial-gradient(#2D3748 1px, transparent 1px); background-size: 28px 28px;"></div>
</div>
<!-- MAIN HEADER: compact fixed top-right (no floating wide bar) -->
<header class="fixed top-3 right-3 z-50">
<div class="k-glass rounded-full px-3 py-1.5 flex items-center gap-2 shadow-card">

<a href="#" class="flex items-center gap-1.5 group shrink-0">
<div class="w-7 h-7 rounded-full bg-gradient-to-tr from-kpink-400 via-kpink-300 to-kpink-200 flex items-center justify-center text-white font-black text-[10px] shadow-sm group-hover:scale-105 transition-transform">
IY
</div>
<span class="font-extrabold tracking-tight text-sm text-ktext-primary">
IYKYK <span class="text-[9px] font-medium px-1.5 py-0.5 rounded-full bg-kpink-50 text-kpink-600 border border-kpink-200">Ticket</span>
</span>
</a>
<div class="flex items-center gap-1.5">
<select id="language-picker" aria-label="Select language" onchange="setSiteLanguage(this.value)" class="bg-white/90 border border-kpink-200 rounded-full px-2 py-1 text-[11px] font-semibold text-ktext-primary focus:outline-none focus:ring-2 focus:ring-kpink-300 cursor-pointer shadow-sm">
<option value="zh">中文</option>
<option value="en">EN</option>
<option value="ko">한국어</option>
<option value="ja">日本語</option>
</select>
<button onclick="scrollToSection('concerts')" class="bg-gradient-to-r from-kpink-400 to-kpink-500 hover:from-kpink-500 hover:to-kpink-600 text-white font-semibold text-[11px] px-3.5 py-1.5 rounded-full shadow-soft hover:shadow-soft-lg transition-all">
<span data-i18n="btnBook">立即预订</span>
</button>
</div>
</div>
</header>
<!-- MAIN CONTENT -->
<main class="flex-grow z-10 max-w-6xl mx-auto px-4 sm:px-6 pt-16 pb-6 space-y-6">
<!-- SERVICE NOTICE BANNER (text only, no box) -->
<div class="max-w-5xl mx-auto text-[9px] sm:text-[10px] text-ktext-primary flex items-start gap-1 mb-1 leading-snug" role="note" id="service-notice">
<strong class="font-bold text-kpink-600 shrink-0" data-i18n="noticeTitle">限量预约服务</strong>
<span data-i18n="noticeBody">：目前仅接受少量购票协助申请。提交预约后请添加微信客服 Chloe_ii0514 确认是否接单、最终报价及退款条款；未经确认请勿付款。预约信息目前仅保存在提交者浏览器中，团队不会自动收到。</span>
</div>
<!-- HERO SECTION -->
<section class="relative pt-0 pb-4 text-center flex flex-col items-center justify-center">
<div class="w-full flex items-center justify-center gap-1.5 px-3 py-1 rounded-none bg-white/90 border border-kpink-200 text-[9px] sm:text-[10px] font-semibold text-kpink-600 shadow-sm mb-3 animate-float-slow">
<span class="w-1.5 h-1.5 rounded-full bg-kpink-400 animate-ping shrink-0"></span>
<span data-i18n="heroBadge">IYKYK / 韩国本土预售优先抢订服务</span>
</div>
<h1 class="text-3xl sm:text-5xl md:text-6xl font-black tracking-tight text-ktext-primary max-w-3xl leading-tight mb-3" data-i18n="heroTitle1">
直通韩国本土优先预售通道
</h1>
<h2 class="text-2xl sm:text-4xl md:text-5xl font-black tracking-tight bg-clip-text text-transparent bg-gradient-to-r from-kpink-500 via-kpink-400 to-rose-400 max-w-3xl leading-tight mb-6" data-i18n="heroTitle2">
安全·透明·极速抢占优质席位
</h2>
<p class="text-xs sm:text-sm md:text-base text-ktext-secondary max-w-2xl font-normal leading-relaxed mb-8" data-i18n="heroDesc">
由专业团队提供韩国本土实名认证账号与优先开售抢订支持。绕过 Global 通道漫长等候与天价黄牛，采用“抢到后付服务费 / 未成功定金全退”安全保障机制。
</p>
<!-- Value Highlights -->
<div class="grid grid-cols-2 sm:grid-cols-4 gap-3 sm:gap-4 w-full max-w-3xl mb-8">
<div class="k-glass p-4 rounded-3xl text-center shadow-card hover:border-kpink-300 transition-all">
<div class="w-8 h-8 mx-auto mb-2 rounded-full bg-kpink-50 flex items-center justify-center text-kpink-500">
<i data-lucide="shield-check" class="w-4 h-4"></i>
</div>
<div class="text-xs font-bold text-ktext-primary" data-i18n="v1Title">成功后再付尾款</div>
<div class="text-[11px] text-ktext-light mt-0.5" data-i18n="v1Sub">第三方托管低风险</div>
</div>
<div class="k-glass p-4 rounded-3xl text-center shadow-card hover:border-kpink-300 transition-all">
<div class="w-8 h-8 mx-auto mb-2 rounded-full bg-kpink-50 flex items-center justify-center text-kpink-500">
<i data-lucide="zap" class="w-4 h-4"></i>
</div>
<div class="text-xs font-bold text-ktext-primary" data-i18n="v2Title">本土提前优先购票</div>
<div class="text-[11px] text-ktext-light mt-0.5" data-i18n="v2Sub">优先抢占内场与VIP</div>
</div>
<div class="k-glass p-4 rounded-3xl text-center shadow-card hover:border-kpink-300 transition-all">
<div class="w-8 h-8 mx-auto mb-2 rounded-full bg-kpink-50 flex items-center justify-center text-kpink-500">
<i data-lucide="user-check" class="w-4 h-4"></i>
</div>
<div class="text-xs font-bold text-ktext-primary" data-i18n="v3Title">在韩实名认证账号</div>
<div class="text-[11px] text-ktext-light mt-0.5" data-i18n="v3Sub">避开海外 IP 排队限制</div>
</div>
<div class="k-glass p-4 rounded-3xl text-center shadow-card hover:border-kpink-300 transition-all">
<div class="w-8 h-8 mx-auto mb-2 rounded-full bg-kpink-50 flex items-center justify-center text-kpink-500">
<i data-lucide="sparkles" class="w-4 h-4"></i>
</div>
<div class="text-xs font-bold text-ktext-primary" data-i18n="v4Title">费用明细公开透明</div>
<div class="text-[11px] text-ktext-light mt-0.5" data-i18n="v4Sub">服务费 10%-15% 起</div>
</div>
</div>
<!-- Active Status Line -->
<div class="bg-white/90 border border-kpink-200 shadow-soft rounded-full px-5 py-2.5 flex items-center gap-3 text-xs text-ktext-secondary">
<span class="flex h-2.5 w-2.5 relative">
<span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-emerald-400 opacity-75"></span>
<span class="relative inline-flex rounded-full h-2.5 w-2.5 bg-emerald-500"></span>
</span>
<span><span data-i18n="statusLabel">当前本土预售通道运行中：</span><strong class="text-ktext-primary font-bold">CHENLE / NCT WISH / aespa / CHANYEOL</strong> <span data-i18n="statusSuffix">等演出接单中</span></span>
</div>
</section>
<!-- SECTION 1: CONCERT SCHEDULE & BOOKING HUB -->
<section id="concerts" class="space-y-6">
<div class="flex flex-col md:flex-row md:items-end justify-between gap-4">
<div>
<div class="text-xs font-bold text-kpink-500 uppercase tracking-wider mb-1 flex items-center gap-1">
Live Concert Schedule
</div>
<h2 class="text-2xl sm:text-3xl font-extrabold text-ktext-primary" data-i18n="concertsHeader">热门演出与代抢预订列表</h2>
<p class="text-xs sm:text-sm text-ktext-secondary mt-1" data-i18n="concertsSubHeader">
同步韩国本土 (KR Page) 与全球 (Global Page) 官方预售节点
</p>
</div>
<div class="flex flex-wrap items-center gap-2 w-full md:w-auto">
<div class="relative flex-grow sm:flex-grow-0">
<i data-lucide="search" class="w-3.5 h-3.5 text-ktext-light absolute left-3 top-1/2 -translate-y-1/2"></i>
<input type="text" id="concert-search" oninput="filterConcerts()" placeholder="搜索艺人/场地..." data-i18n-placeholder="searchPlaceholder" class="w-full sm:w-56 bg-white/90 border border-kpink-200 rounded-full pl-9 pr-4 py-1.5 text-xs text-ktext-primary focus:outline-none focus:ring-2 focus:ring-kpink-300">
</div>

<div class="flex items-center gap-1.5 bg-white/80 p-1 rounded-full border border-kpink-100 text-xs font-semibold">
<button onclick="setCategoryFilter('all')" id="tab-all" class="concert-tab bg-kpink-400 text-white px-3.5 py-1 rounded-full transition-all shadow-sm" data-i18n="tabAll">全部</button>
<button onclick="setCategoryFilter('dome')" id="tab-dome" class="concert-tab text-ktext-secondary hover:text-ktext-primary px-3.5 py-1 rounded-full transition-all" data-i18n="tabDome">大型/Dome</button>
<button onclick="setCategoryFilter('fanmeeting')" id="tab-fanmeeting" class="concert-tab text-ktext-secondary hover:text-ktext-primary px-3.5 py-1 rounded-full transition-all" data-i18n="tabFM">FM/Party</button>
</div>
</div>
</div>
<div id="concert-grid" class="grid grid-cols-1 md:grid-cols-2 gap-6">
<!-- Injected via JS -->
</div>
</section>
<!-- SECTION 2: SERVICE PLANS -->
<section id="services" class="space-y-6">
<div class="text-center space-y-2 max-w-xl mx-auto">
<span class="text-xs font-bold text-kpink-500 uppercase tracking-wider">Transparent Service Plans</span>
<h2 class="text-2xl sm:text-3xl font-extrabold text-ktext-primary" data-i18n="plansHeader">选择最适合您的代抢服务方案</h2>
<p class="text-xs sm:text-sm text-ktext-secondary" data-i18n="plansSubHeader">
包含本土实名认证账号使用权、抢订操作及全程票务对接指导
</p>
</div>
<div class="grid grid-cols-1 md:grid-cols-2 gap-6">
<!-- Plan A -->
<div class="k-glass rounded-4xl p-6 sm:p-8 border-2 border-kpink-300 relative shadow-soft flex flex-col justify-between space-y-6">
<div class="absolute -top-3.5 right-6 bg-gradient-to-r from-kpink-400 to-kpink-500 text-white text-xs font-semibold px-4 py-1 rounded-full shadow-sm">
<span data-i18n="planABadge">限量预约 · 客服确认后付款</span>
</div>
<div class="space-y-4">
<div class="w-10 h-10 rounded-2xl bg-kpink-100 flex items-center justify-center text-kpink-600">
<i data-lucide="shield-check" class="w-5 h-5"></i>
</div>
<div>
<h3 class="text-lg font-bold text-ktext-primary" data-i18n="planATitle">抢到后付模式 (Success-First)</h3>
<p class="text-xs text-ktext-secondary mt-1" data-i18n="planADesc">资金安全优先，出票成功后再付主体服务费</p>
</div>
<div class="text-2xl font-black text-kpink-600">
<span data-i18n="depositLine">定金 ¥100</span> <span class="text-xs font-normal text-ktext-secondary" data-i18n="depositLineSub">+ 服务费 10%–20%（定金抵扣最终费用）</span>
</div>
<ul class="text-xs text-ktext-secondary space-y-2.5 pt-2">
<li class="flex items-center gap-2">
<i data-lucide="check" class="w-4 h-4 text-emerald-500 shrink-0"></i>
<span data-i18n="planA1">分配专人韩国本土实名认证账号</span>
</li>
<li class="flex items-center gap-2">
<i data-lucide="check" class="w-4 h-4 text-emerald-500 shrink-0"></i>
<span data-i18n="planA2">抢票未成功：¥100 定金全额退还</span>
</li>
<li class="flex items-center gap-2">
<i data-lucide="check" class="w-4 h-4 text-emerald-500 shrink-0"></i>
<span data-i18n="planA3">成功出票后支付剩余款项，已付 ¥100 定金抵扣最终应付金额</span>
</li>
</ul>
</div>
<button onclick="openBookingModal('Success-First')" class="w-full bg-gradient-to-r from-kpink-400 to-kpink-500 hover:from-kpink-500 hover:to-kpink-600 text-white font-bold py-3.5 rounded-full text-xs shadow-soft transition-all" data-i18n="planBookBtn">
按此方案预订
</button>
</div>
<!-- Plan B -->
<div class="k-glass rounded-4xl p-6 sm:p-8 border border-kpink-200 relative shadow-card flex flex-col justify-between space-y-6">
<div class="space-y-4">
<div class="w-10 h-10 rounded-2xl bg-kpink-100 flex items-center justify-center text-kpink-600">
<i data-lucide="award" class="w-5 h-5"></i>
</div>
<div>
<h3 class="text-lg font-bold text-ktext-primary" data-i18n="planBTitle">VIP 前排锁位方案 (VIP Priority)</h3>
<p class="text-xs text-ktext-secondary mt-1" data-i18n="planBDesc">适合拟冲刺首尔内场 VIP / 极其紧缺席位</p>
</div>
<div class="text-2xl font-black text-ktext-primary">
<span data-i18n="depositLine">定金 ¥100</span> <span class="text-xs font-normal text-ktext-secondary" data-i18n="depositLineSub">+ 服务费 10%–20%（定金抵扣最终费用）</span>
</div>
<ul class="text-xs text-ktext-secondary space-y-2.5 pt-2">
<li class="flex items-center gap-2">
<i data-lucide="check" class="w-4 h-4 text-emerald-500 shrink-0"></i>
<span data-i18n="planB1">优先调配高响应度本土账号组</span>
</li>
<li class="flex items-center gap-2">
<i data-lucide="check" class="w-4 h-4 text-emerald-500 shrink-0"></i>
<span data-i18n="planB2">专属客服一对一全程同步抢票截图</span>
</li>
<li class="flex items-center gap-2">
<i data-lucide="check" class="w-4 h-4 text-emerald-500 shrink-0"></i>
<span data-i18n="planB3">未出票：¥100 定金全额退还</span>
</li>
</ul>
</div>
<button onclick="openBookingModal('VIP-Priority')" class="w-full bg-white hover:bg-kpink-50 border border-kpink-200 text-ktext-primary font-bold py-3.5 rounded-full text-xs transition-all" data-i18n="planBookBtn">
按此方案预订
</button>
</div>
</div>
</section>
<!-- SECTION 3: TRANSPARENT CALCULATOR -->
<section id="calculator" class="k-glass rounded-4xl p-6 sm:p-10 shadow-soft border border-kpink-200">
<div class="max-w-3xl mx-auto space-y-8">
<div class="text-center space-y-2">
<span class="text-xs font-bold text-kpink-500 uppercase tracking-wider">Cost Transparency</span>
<h2 class="text-2xl sm:text-3xl font-extrabold text-ktext-primary" data-i18n="calcHeader">代抢服务费用实时测算</h2>
<p class="text-xs sm:text-sm text-ktext-secondary max-w-xl mx-auto" data-i18n="calcSubHeader">
拒绝黄牛动辄数倍的恶劣溢价。依据官方票面与合理服务费率计算，拒绝隐藏收费。
</p>
</div>

<div class="bg-white/90 rounded-3xl p-6 sm:p-8 border border-kpink-100 shadow-sm space-y-6">
<div class="grid grid-cols-1 sm:grid-cols-2 gap-6">
<div class="space-y-2">
<label class="block text-xs font-semibold text-ktext-primary" data-i18n="calcSelectShow">选择拟代抢演出项目</label>
<select id="calc-show" onchange="updateCalculator()" class="w-full bg-kbg border border-kpink-200 rounded-2xl px-4 py-3 text-xs sm:text-sm text-ktext-primary focus:outline-none focus:ring-2 focus:ring-kpink-300">
<option value="77000" selected>CHENLE / GISELLE / CHANYEOL 生日会 - 77,000 韩元</option>
<option value="165000">NCT WISH (一般席) - 165,000 韩元</option>
<option value="220000">NCT WISH (VIP席) - 220,000 韩元</option>
<option value="121000">aespa FAN MEETING - 121,000 韩元</option>
<option value="143000">AND2BLE FAN-CON - 143,000 韩元</option>
<option value="154000">NMIXX 1ST WORLD TOUR - 154,000 韩元</option>
</select>
</div>
<div class="space-y-2">
<label class="block text-xs font-semibold text-ktext-primary" data-i18n="calcSelectTier">服务档位</label>
<select id="calc-markup" onchange="updateCalculator()" class="w-full bg-kbg border border-kpink-200 rounded-2xl px-4 py-3 text-xs sm:text-sm text-ktext-primary focus:outline-none focus:ring-2 focus:ring-kpink-300">
<option value="0.10" data-i18n-opt="tierBasic">基础档: 10% 服务费 (一般席位/看台)</option>
<option value="0.15" selected data-i18n-opt="tierStd">标准档: 15% 服务费 (热门推荐)</option>
<option value="0.20" data-i18n-opt="tierRush">冲刺档: 20% 服务费 (稀缺前排 VIP)</option>
</select>
</div>
</div>
<div class="pt-4 border-t border-kpink-100">
<div class="grid grid-cols-1 md:grid-cols-3 gap-4 text-center">
<div class="p-4 rounded-2xl bg-gray-50 border border-gray-100 space-y-1">
<div class="text-xs font-bold text-gray-500" data-i18n="calcFaceLabel">官方原票价 (折合RMB)</div>
<div class="text-lg font-bold text-gray-700" id="calc-cost-face">¥ 406</div>
<div class="text-[10px] text-gray-400" data-i18n="calcRateNote">按实时汇率折算</div>
</div>
<div class="p-4 rounded-2xl bg-kpink-50 border-2 border-kpink-300 space-y-1 relative shadow-sm">
<div class="text-xs font-bold text-kpink-600" data-i18n="calcIykykLabel">IYKYK 预估总支出</div>
<div class="text-xl font-extrabold text-kpink-600" id="calc-cost-iykyk">¥ 609</div>
<div class="text-[10px] text-kpink-500 font-semibold" id="calc-fee-detail">含服务费 ¥203</div>
</div>
<div class="p-4 rounded-2xl bg-rose-50/60 border border-rose-100 space-y-1">
<div class="text-xs font-bold text-rose-500" data-i18n="calcScalperLabel">传统二手黄牛参考价</div>
<div class="text-lg font-bold text-rose-600" id="calc-cost-scalper">¥ 812 ~ 1,218</div>
<div class="text-[10px] text-rose-400" data-i18n="calcScalperNote">200%-300% 天价溢价</div>
</div>
</div>
</div>
</div>
</div>
</section>
<!-- SECTION 4: ORDER LOOKUP PORTAL -->
<section id="orders" class="space-y-6">
<div class="text-center space-y-2 max-w-xl mx-auto">
<span class="text-xs font-bold text-kpink-500 uppercase tracking-wider">Real-time Order Tracking</span>
<h2 class="text-2xl sm:text-3xl font-extrabold text-ktext-primary" data-i18n="orderHeader">订单进度查询与状态跟踪</h2>
<p class="text-xs sm:text-sm text-ktext-secondary" data-i18n="orderSubHeader">
输入订单号（如 M4-XXXX 或 IY-2026-8812）或下单时填写的手机/社交账号进行实时检索
</p>
</div>
<div class="max-w-xl mx-auto k-glass p-6 sm:p-8 rounded-4xl border border-kpink-200 shadow-soft space-y-6">
<div class="flex gap-2">
<input type="text" id="search-order-input" placeholder="输入订单号或手机/微信账号" data-i18n-placeholder="orderSearchPlaceholder" class="flex-grow bg-white border border-kpink-200 rounded-2xl px-4 py-3 text-xs sm:text-sm text-ktext-primary focus:outline-none focus:ring-2 focus:ring-kpink-300">
<button onclick="searchOrder()" class="bg-gradient-to-r from-kpink-400 to-kpink-500 text-white font-bold px-6 py-3 rounded-2xl text-xs hover:from-kpink-500 hover:to-kpink-600 transition-all shrink-0" data-i18n="btnQueryStatus">
查询状态
</button>
</div>
<div id="order-result-box" class="hidden bg-white p-5 rounded-3xl border border-kpink-100 space-y-4 shadow-sm">
<div class="flex items-center justify-between border-b border-kpink-100 pb-3">
<div>
<span class="text-xs font-bold text-ktext-primary" id="res-order-id">#IY-2026-8812</span>
<div class="text-[11px] text-ktext-secondary" id="res-show-title">2026 CHENLE B-day PARTY [Lele’s Show 2]</div>
</div>
<span class="text-xs font-semibold px-3 py-1 rounded-full bg-kpink-100 text-kpink-600" id="res-status-badge" data-i18n="defaultBadge">
YES24 本土实名账号锁定中
</span>
</div>
<div class="space-y-3 text-xs">
<div class="flex items-start gap-3">
<div class="w-5 h-5 rounded-full bg-emerald-500 text-white flex items-center justify-center text-[10px] font-bold shrink-0 mt-0.5">✓</div>
<div>
<div class="font-bold text-ktext-primary" data-i18n="step1Title">抢票需求提交与方案锁定</div>
<div class="text-[10px] text-ktext-light" data-i18n="step1Desc">客户信息提交成功，第三方退订担保生效</div>
</div>
</div>
<div class="flex items-start gap-3">
<div class="w-5 h-5 rounded-full bg-emerald-500 text-white flex items-center justify-center text-[10px] font-bold shrink-0 mt-0.5">✓</div>
<div>
<div class="font-bold text-ktext-primary" data-i18n="step2Title">本土实名认证账号完成匹配</div>
<div class="text-[10px] text-ktext-light" data-i18n="step2Desc">已分发首尔本土高响应 YES24 账号</div>
</div>
</div>
<div class="flex items-start gap-3">
<div class="w-5 h-5 rounded-full bg-kpink-400 text-white flex items-center justify-center text-[10px] font-bold shrink-0 mt-0.5 animate-pulse">3</div>
<div>
<div class="font-bold text-kpink-600" data-i18n="step3Title">等待韩国本土预售窗口开启</div>
<div class="text-[10px] text-ktext-secondary" data-i18n="step3Desc">抢票人员已准备完毕，预计开售即刻进入抢订</div>
</div>
</div>
<div class="flex items-start gap-3 opacity-40">
<div class="w-5 h-5 rounded-full bg-gray-200 text-gray-500 flex items-center justify-center text-[10px] font-bold shrink-0 mt-0.5">4</div>
<div>
<div class="font-bold text-ktext-primary" data-i18n="step4Title">出票凭证确认与尾款结算</div>
<div class="text-[10px] text-ktext-light" data-i18n="step4Desc">发送官方订票截图与实体/电子票查验</div>
</div>
</div>
</div>

</div>
</div>
</section>
<!-- SECTION 5: TRUST & GUARANTEES -->
<section id="trust" class="space-y-8">
<div class="text-center space-y-2">
<span class="text-xs font-bold text-kpink-500 uppercase tracking-wider">Safety & Service Protocol</span>
<h2 class="text-2xl sm:text-3xl font-extrabold text-ktext-primary" data-i18n="trustHeader">服务保障与隐私承诺</h2>
</div>
<div class="grid grid-cols-1 md:grid-cols-3 gap-6">
<div class="k-glass p-6 rounded-3xl space-y-3 border border-kpink-200 shadow-card">
<div class="w-10 h-10 rounded-2xl bg-kpink-100 flex items-center justify-center text-kpink-600">
<i data-lucide="lock" class="w-5 h-5"></i>
</div>
<h3 class="font-bold text-sm text-ktext-primary" data-i18n="t1Title">严格个人信息保护</h3>
<p class="text-xs text-ktext-secondary leading-relaxed" data-i18n="t1Desc">
客户所有身份证照及观演人信息仅用于本次门票实名绑定与官方查验，抢票结束后即刻清空，绝不留存。
</p>
</div>
<div class="k-glass p-6 rounded-3xl space-y-3 border border-kpink-200 shadow-card">
<div class="w-10 h-10 rounded-2xl bg-kpink-100 flex items-center justify-center text-kpink-600">
<i data-lucide="user-check" class="w-5 h-5"></i>
</div>
<h3 class="font-bold text-sm text-ktext-primary" data-i18n="t2Title">真实本土合规账号</h3>
<p class="text-xs text-ktext-secondary leading-relaxed" data-i18n="t2Desc">
仅使用在韩留学生持有之本土实名认证账号，避免海外网络封锁，合规抢订，杜绝非法外挂脚本导致的封号风险。
</p>
</div>
<div class="k-glass p-6 rounded-3xl space-y-3 border border-kpink-200 shadow-card">
<div class="w-10 h-10 rounded-2xl bg-kpink-100 flex items-center justify-center text-kpink-600">
<i data-lucide="refresh-cw" class="w-5 h-5"></i>
</div>
<h3 class="font-bold text-sm text-ktext-primary" data-i18n="t3Title">未出票 100% 全额退款</h3>
<p class="text-xs text-ktext-secondary leading-relaxed" data-i18n="t3Desc">
若因席位极度紧缺导致未能成功出票，所有定金无条件原路退回，并提供二次转让防诈鉴别指导。
</p>
</div>
</div>
</section>
</main>
<!-- FOOTER -->
<footer class="mt-20 bg-white/80 border-t border-kpink-200 py-8 text-center text-xs text-ktext-light z-10 relative">
<div class="max-w-6xl mx-auto px-4 space-y-3">
<div class="flex items-center justify-center gap-2 font-bold text-ktext-primary text-sm">
<span class="w-2 h-2 rounded-full bg-kpink-400"></span>
IYKYK Ticket Platform
</div>
<p class="max-w-xl mx-auto leading-relaxed text-[11px] text-ktext-secondary">
IYKYK 为海外粉丝提供韩国演唱会本土优先预售协助、抢订及全程协助服务。演出日程及票价来源于 2026 官方公布数据。
</p>
<p class="text-[10px] text-ktext-light">
© 2026 IYKYK Team. All rights reserved.
</p>
<button onclick="openAdminLogin()" class="mt-2 inline-flex items-center gap-1 bg-gray-100 hover:bg-gray-200 text-gray-400 hover:text-gray-600 font-medium text-[10px] px-3 py-1.5 rounded-full border border-gray-200 transition-all cursor-pointer">
<svg xmlns="http://www.w3.org/2000/svg" width="10" height="10" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round"><rect width="18" height="11" x="3" y="11" rx="2" ry="2"/><path d="M7 11V7a5 5 0 0 1 10 0v4"/></svg>
管理员后台
</button>
</div>
</footer>
<!-- ADMIN LOGIN MODAL -->
<div id="admin-login-modal" class="fixed inset-0 bg-black/40 backdrop-blur-sm z-[60] hidden items-center justify-center p-4">
<div class="bg-white w-full max-w-xs rounded-3xl p-6 shadow-2xl space-y-4">
<div class="text-center space-y-1">
<div class="w-10 h-10 mx-auto rounded-full bg-kpink-100 flex items-center justify-center text-kpink-500">
<i data-lucide="lock" class="w-5 h-5"></i>
</div>
<h3 class="text-sm font-bold text-ktext-primary">管理员验证</h3>
<p class="text-[10px] text-ktext-light">请输入管理密码以查看预约记录</p>
</div>
<div class="space-y-2">
<input type="password" id="admin-pwd-input" onkeydown="if(event.key==='Enter')verifyAdmin()" placeholder="管理密码" class="w-full bg-kbg border border-kpink-200 rounded-2xl px-4 py-2.5 text-sm text-ktext-primary focus:outline-none focus:ring-2 focus:ring-kpink-300 text-center tracking-widest">
<p id="admin-pwd-error" class="text-[10px] text-red-500 text-center hidden">密码错误，请重试</p>
</div>
<div class="flex gap-2">
<button onclick="closeAdminLogin()" class="flex-1 bg-gray-100 hover:bg-gray-200 text-ktext-secondary font-semibold py-2 rounded-full text-xs transition-all">取消</button>
<button onclick="verifyAdmin()" class="flex-1 bg-gradient-to-r from-kpink-400 to-kpink-500 hover:from-kpink-500 hover:to-kpink-600 text-white font-semibold py-2 rounded-full text-xs transition-all">进入</button>
</div>
</div>
</div>
<!-- INTERACTIVE BOOKING MODAL -->
<div id="booking-modal" class="fixed inset-0 bg-black/40 backdrop-blur-sm z-50 flex items-center justify-center p-4 opacity-0 pointer-events-none transition-opacity duration-300">
<div class="bg-white w-full max-w-lg rounded-4xl p-6 sm:p-8 shadow-2xl space-y-6 transform scale-95 transition-transform duration-300 max-h-[90vh] overflow-y-auto" id="modal-card">
<div class="flex items-center justify-between border-b border-kpink-100 pb-4">
<div class="flex items-center gap-2">
<div class="w-8 h-8 rounded-full bg-gradient-to-tr from-kpink-400 to-kpink-200 text-white font-bold text-xs flex items-center justify-center">
IY
</div>
<span class="font-bold text-base text-ktext-primary" data-i18n="modalTitle">预订代抢服务</span>
</div>
<button onclick="closeBookingModal()" class="text-ktext-light hover:text-ktext-primary p-1">
<i data-lucide="x" class="w-5 h-5"></i>
</button>
</div>
<!-- Form -->
<form id="booking-form" onsubmit="submitBooking(event)" class="space-y-4 text-xs">
<div class="space-y-1.5">
<label class="font-semibold text-ktext-primary" data-i18n="f1">1. 选择演出项目</label>
<select id="dw-show" onchange="updateModalPrice()" class="w-full bg-kbg border border-kpink-200 rounded-2xl px-4 py-3 text-ktext-primary focus:outline-none focus:ring-2 focus:ring-kpink-300">
<option value="2026 CHENLE B-day PARTY [Lele’s Show 2]" data-price="77000" data-price-vip="77000" data-price-general="77000">2026 CHENLE B-day PARTY [Lele’s Show 2]</option>
<option value="NCT WISH 2nd CONCERT TOUR" data-price="165000" data-price-vip="220000" data-price-general="165000">NCT WISH 2nd CONCERT TOUR (高尺巨蛋)</option>
<option value="2026 aespa FAN MEETING" data-price="121000" data-price-vip="121000" data-price-general="121000">2026 aespa FAN MEETING (高丽大华正)</option>
<option value="2026 GISELLE B-day PARTY" data-price="77000" data-price-vip="77000" data-price-general="77000">2026 GISELLE B-day PARTY (明和Live Hall)</option>
<option value="2026 AND2BLE FAN-CON" data-price="143000" data-price-vip="143000" data-price-general="143000">2026 AND2BLE FAN-CON (Tiger Dome)</option>
<option value="2026 SUNWOO 粉丝见面会" data-price="99000" data-price-vip="99000" data-price-general="99000">2026 SUNWOO 粉丝见面会《UNCHAINED》</option>
<option value="2026 CLOSE YOUR EYES FANCON" data-price="121000" data-price-vip="121000" data-price-general="99000">2026 CLOSE YOUR EYES FANCON</option>
<option value="NMIXX 1ST WORLD TOUR INCHEON" data-price="154000" data-price-vip="154000" data-price-general="154000">NMIXX 1ST WORLD TOUR FINALE</option>
<option value="2026 CHANYEOL B-day PARTY" data-price="77000" data-price-vip="77000" data-price-general="77000">2026 CHANYEOL B-day PARTY</option>
</select>
</div>
<div class="grid grid-cols-2 gap-3">
<div class="space-y-1.5">
<label class="font-semibold text-ktext-primary" data-i18n="f2">2. 席位偏好</label>
<select id="dw-tier" onchange="updateModalPrice()" class="w-full bg-kbg border border-kpink-200 rounded-2xl px-3 py-3 text-ktext-primary focus:outline-none focus:ring-2 focus:ring-kpink-300">
<option value="VIP 席位 / 内场前排" data-i18n-opt="tierVip">VIP 席位 / 内场前排</option>
<option value="指定席 / 一般看台" data-i18n-opt="tierGeneral">指定席 / 一般看台</option>
<option value="任意可接受席位" data-i18n-opt="tierAny">任意可接受席位</option>
</select>
</div>
<div class="space-y-1.5">
<label class="font-semibold text-ktext-primary" data-i18n="f3">3. 张数</label>
<select id="dw-qty" onchange="updateModalPrice()" class="w-full bg-kbg border border-kpink-200 rounded-2xl px-3 py-3 text-ktext-primary focus:outline-none focus:ring-2 focus:ring-kpink-300">
<option value="1" data-i18n-opt="qty1">1 张</option>
<option value="2" data-i18n-opt="qty2">2 张</option>
</select>

</div>
</div>
<div class="space-y-1.5">
<label class="font-semibold text-ktext-primary" data-i18n="f4">4. 付费服务方案</label>
<select id="dw-plan" onchange="updateModalPrice()" class="w-full bg-kbg border border-kpink-200 rounded-2xl px-4 py-3 text-ktext-primary focus:outline-none focus:ring-2 focus:ring-kpink-300">
<option value="Success-First" data-i18n-opt="planSuccess">成功后付款（需客服确认接单）</option>
<option value="VIP-Priority" data-i18n-opt="planVip">优先服务咨询（需客服确认接单）</option>
</select>
</div>
<div class="space-y-1.5">
<label class="font-semibold text-ktext-primary" data-i18n="f5">5. 昵称（请勿填写证件姓名）</label>
<input type="text" id="dw-name" placeholder="如：K-pop fan" data-i18n-placeholder="nickPlaceholder" class="w-full bg-kbg border border-kpink-200 rounded-2xl px-4 py-3 text-ktext-primary placeholder:text-ktext-light focus:outline-none focus:ring-2 focus:ring-kpink-300">
</div>
<div class="space-y-1.5">
<label class="font-semibold text-ktext-primary" data-i18n="f6">6. 联系方式（可选；请勿填写证件或支付信息）</label>
<input type="text" id="dw-contact" placeholder="可留微信或邮箱；请勿提供敏感信息" data-i18n-placeholder="contactPlaceholder" class="w-full bg-kbg border border-kpink-200 rounded-2xl px-4 py-3 text-ktext-primary placeholder:text-ktext-light focus:outline-none focus:ring-2 focus:ring-kpink-300">
</div>
<!-- Price Summary Box -->
<div class="p-4 rounded-2xl bg-kpink-50/80 border border-kpink-200 space-y-1.5">
<div class="flex justify-between items-center text-xs">
<span class="text-ktext-secondary" data-i18n="faceLabel">票面估算：</span>
<span class="font-bold text-ktext-primary" id="dw-face-val">¥ 406</span>
</div>
<div class="flex justify-between items-center text-xs">
<span class="text-ktext-secondary" data-i18n="feeLabel">服务费及费用明细：</span>
<span class="font-bold text-kpink-600 text-sm" id="dw-deposit-val">服务费按 10%–20% 计算</span>
</div>
<div class="text-[10px] text-ktext-light pt-1 border-t border-kpink-200/60" data-i18n="depositNote">
* 定金 ¥100 可抵扣最终费用，并非额外收费；抢票失败全额退还定金。少量接单，实际票价、库存、服务费及付款时机以客服书面确认为准。请勿在客服确认前付款。
</div>
</div>
<p class="text-xs text-amber-800 bg-amber-50 border border-amber-200 p-3 rounded-xl" data-i18n="modalWarning">⚠️ 限量人工接单：提交仅代表预约申请，不代表已接单、已付款或已购票。受邀朋友请使用 <strong>?test=1</strong> 测试链接，不要付款。请核实实名制及官方售票平台规则。</p>
<button type="submit" class="w-full bg-gradient-to-r from-kpink-400 to-kpink-500 hover:from-kpink-500 hover:to-kpink-600 text-white font-bold py-3.5 rounded-full shadow-soft hover:shadow-soft-lg transition-all text-sm flex items-center justify-center gap-2">
<span data-i18n="btnSubmitBooking">提交预约申请 · 联系客服确认</span>
<i data-lucide="arrow-right" class="w-4 h-4"></i>
</button>
</form>
</div>
</div>
<!-- POST-BOOKING CONTACT & PAYMENT INFORMATION -->
<div id="after-booking-modal" role="dialog" aria-modal="true" aria-labelledby="after-booking-title" class="fixed inset-0 bg-black/50 backdrop-blur-sm z-[60] hidden items-center justify-center p-4">
<div class="bg-white w-full max-w-xl rounded-3xl p-5 sm:p-7 shadow-2xl max-h-[90vh] overflow-y-auto space-y-4">
<div class="flex justify-between items-center">
<h2 id="after-booking-title" class="text-xl font-bold text-ktext-primary" data-i18n="afterTitle">💗 预约申请已提交（待人工确认）</h2>
<button onclick="closeAfterBooking()" aria-label="关闭" class="text-2xl text-gray-500 hover:text-gray-800">×</button>
</div>
<p class="text-sm text-ktext-secondary"><span data-i18n="afterRef">预约编号：</span><strong id="after-booking-id" class="text-kpink-600 font-bold"></strong> <button onclick="copyBookingId()" class="underline text-kpink-600 ml-1 font-semibold" data-i18n="copyBtn">复制</button></p>
<div class="rounded-2xl bg-kpink-50 border border-kpink-200 p-4 text-sm leading-6">
<strong data-i18n="step1Header">第一步：添加微信客服 Chloe_ii0514</strong>
<p data-i18n="step1Text">请主动添加客服并发送预约编号、演唱会和场次，确认是否还有少量服务名额、票价、¥100 可抵扣定金、10%–20% 服务费、实名入场规则及退款条件。</p>
<div class="flex gap-2 items-center mt-3">
<code class="font-bold bg-white px-3 py-1 rounded-lg border border-kpink-200 text-kpink-700">Chloe_ii0514</code>
<button onclick="navigator.clipboard?.writeText('Chloe_ii0514').then(()=>showToast('微信号已复制'))" class="px-3.5 py-1 bg-white hover:bg-kpink-100 text-xs font-semibold rounded-full border border-kpink-300 transition-colors" data-i18n="copyWechat">复制微信号</button>
</div>
</div>
<div class="rounded-2xl border border-amber-200 bg-amber-50 p-3.5 text-xs leading-5 text-amber-900" data-i18n="payWarning">
付款前请注意：当前仅接受少量购票协助申请。预约并不保证抢票成功。请先通过微信客服确认接单、最终费用、付款条件及退款规则，未经客服确认请勿转账。请核实收款方名称与客服提供的信息一致。本站不会自动验证付款，付款后需由客服人工核实。
</div>
<div class="rounded-2xl border border-kpink-200 p-3.5 text-xs bg-kpink-50">
<span data-i18n="m4TestNote">📋 M4 测试说明：如果你是受邀体验流程的朋友，请使用网址参数 ?test=1 进入测试模式。测试预约不代表真实购票需求，请勿付款。</span> <span id="m4-storage-note"></span>
</div>
<button onclick="recordWechatClick()" class="w-full rounded-full border border-kpink-300 bg-white hover:bg-kpink-50 py-3 font-semibold text-kpink-600 transition-all text-xs sm:text-sm shadow-sm" data-i18n="intentBtn">我已复制微信号 · 记录客服意向</button>
<h3 class="font-bold text-ktext-primary text-sm pt-2" data-i18n="step2Header">第二步：客服确认后选择支付方式</h3>
<label class="flex items-start gap-2.5 text-xs text-ktext-secondary cursor-pointer">
<input type="checkbox" id="payment-unlock" onchange="togglePayment()" class="mt-0.5 rounded text-kpink-500 focus:ring-kpink-400">
<span data-i18n="checkLabel">我确认已与客服沟通，核实了接单能力、实名入场要求、最终报价及退款条款。</span>
</label>
<!-- Payment QRs -->
<div id="payment-options" class="grid grid-cols-1 sm:grid-cols-2 gap-4 hidden pt-2">
<div class="border border-blue-200 bg-blue-50/30 rounded-2xl p-4 text-center">
<h4 class="font-bold text-blue-600 mb-2 text-xs">支付宝 Alipay</h4>
<div class="bg-white p-2 rounded-xl border border-blue-100 inline-block shadow-sm">
<svg class="w-44 h-44 mx-auto" viewBox="0 0 200 200" fill="none" xmlns="http://www.w3.org/2000/svg">
<rect width="200" height="200" rx="12" fill="white"/>
<path d="M20 20H80V80H20V20ZM35 35V65H65V35H35ZM42.5 42.5H57.5V57.5H42.5V42.5Z" fill="#1677FF"/>
<path d="M120 20H180V80H120V20ZM135 35V65H165V35H135ZM142.5 42.5H157.5V57.5H142.5V42.5Z" fill="#1677FF"/>
<path d="M20 120H80V180H20V120ZM35 135V165H65V135H35ZM42.5 142.5H57.5V157.5H42.5V142.5Z" fill="#1677FF"/>
<rect x="90" y="20" width="15" height="15" fill="#1677FF"/>
<rect x="90" y="50" width="15" height="40" fill="#1677FF"/>
<rect x="120" y="90" width="60" height="15" fill="#1677FF"/>
<rect x="100" y="120" width="30" height="30" fill="#1677FF"/>
<rect x="140" y="140" width="40" height="40" fill="#1677FF"/>
<rect x="20" y="90" width="50" height="15" fill="#1677FF"/>
</svg>
</div>
<div class="text-[11px] text-blue-800 font-semibold mt-2">sweetwiee_C0(**琳)</div>
</div>
<div class="border border-emerald-200 bg-emerald-50/30 rounded-2xl p-4 text-center">
<h4 class="font-bold text-emerald-600 mb-2 text-xs">微信支付 WeChat Pay</h4>
<div class="bg-white p-2 rounded-xl border border-emerald-100 inline-block shadow-sm">
<svg class="w-44 h-44 mx-auto" viewBox="0 0 200 200" fill="none" xmlns="http://www.w3.org/2000/svg">
<rect width="200" height="200" rx="12" fill="white"/>
<path d="M20 20H80V80H20V20ZM35 35V65H65V35H35ZM42.5 42.5H57.5V57.5H42.5V42.5Z" fill="#07C160"/>
<path d="M120 20H180V80H120V20ZM135 35V65H165V35H135ZM142.5 42.5H157.5V57.5H142.5V42.5Z" fill="#07C160"/>
<path d="M20 120H80V180H20V120ZM35 135V165H65V135H35ZM42.5 142.5H57.5V157.5H42.5V142.5Z" fill="#07C160"/>
<rect x="90" y="30" width="20" height="30" fill="#07C160"/>
<rect x="130" y="90" width="30" height="20" fill="#07C160"/>
<rect x="90" y="130" width="40" height="40" fill="#07C160"/>
<rect x="150" y="120" width="30" height="50" fill="#07C160"/>
<rect x="100" y="90" width="20" height="20" fill="#07C160"/>

</svg>
</div>
<div class="text-[11px] text-emerald-800 font-semibold mt-2">Syniiec0oo(**琳)</div>
</div>
</div>
<p class="text-[11px] text-ktext-light" data-i18n="payTip">提示：以上为扫码收款示例码，并非自动跳转的支付链接；请在付款前核实收款账户。无需向网站提交付款密码或证件照片。</p>
<button onclick="closeAfterBooking()" class="w-full bg-kpink-500 hover:bg-kpink-600 text-white rounded-full py-3 font-bold transition-colors text-xs sm:text-sm" data-i18n="gotIt">我知道了</button>
</div>
</div>
<!-- TOAST NOTIFICATION -->
<div id="toast" class="fixed bottom-6 right-6 bg-white/95 border border-kpink-300 px-5 py-3 rounded-2xl shadow-soft text-xs font-semibold text-ktext-primary flex items-center gap-3 opacity-0 pointer-events-none transition-all duration-300 z-50">
<span class="w-2 h-2 rounded-full bg-kpink-500 animate-ping"></span>
<span id="toast-message">提示信息</span>
</div>
<!-- JAVASCRIPT LOGIC -->
<script>
const concertData = [
{
id: 1,
category: "fanmeeting",
title: "2026 CHENLE B-day PARTY [Lele’s Show 2]",
venue: "YES24 LIVE HALL (首尔)",
priceKRW: "全席统一 77,000 韩元",
priceRMB: "~ ¥406 RMB",
krPresale: "2026.10.27 (周二) 8:00 PM (KST)",
globalPresale: "2026.10.28 (周三) 8:00 PM (KST)",
status: "YES24独占 · 预订中",
tag: "NCT DREAM · 生日Party"
},
{
id: 2,
category: "dome",
title: "NCT WISH 2nd CONCERT TOUR 'INTO THE WISH' IN SEOUL",
venue: "GOCHEOK SKY DOME (首尔高尺巨蛋)",
priceKRW: "VIP席 220,000 / 一般席 165,000 韩元",
priceRMB: "~ ¥1,160 / ¥870 RMB",
krPresale: "2026.11.02 (周一) 8:00 PM (KST)",
globalPresale: "2026.11.03 (周二) 8:00 PM (KST)",
status: "火热预订中",
tag: "高尺巨蛋 · 顶级热度"
},
{
id: 3,
category: "fanmeeting",
title: "2026 aespa FAN MEETING “MY 보고싶다 ae가”",
venue: "高丽大学华正体育馆 (Tiger Dome)",
priceKRW: "指定席 121,000 韩元",
priceRMB: "~ ¥638 RMB",
krPresale: "2026.10.27 (周二) 8:00 PM (KST)",
globalPresale: "2026.10.28 (周三) 8:00 PM (KST)",
status: "热抢中",
tag: "粉丝见面会 · 席位紧缺"
},
{
id: 4,
category: "fanmeeting",
title: "2026 GISELLE B-day PARTY [In MY Blood]",
venue: "明和 Live Hall (MYUNGHWA LIVE HALL)",
priceKRW: "全席统一 77,000 韩元",
priceRMB: "~ ¥406 RMB",
krPresale: "2026.10.21 (周三) 8:00 PM (KST)",
globalPresale: "无 Global 通道 (仅本土独占)",
status: "本土独占",
tag: "生日Party · LiveHouse"
},
{
id: 5,
category: "fanmeeting",
title: "2026 AND2BLE FAN-CON <W!nter inside> In Seoul",
venue: "Hwajeong Tiger Dome (华正体育馆)",
priceKRW: "全席统一 143,000 韩元",
priceRMB: "~ ¥755 RMB",
krPresale: "2026.10.21 (周三) 8:00 PM (KST)",
globalPresale: "2026.10.22 (周四) 8:00 PM (KST)",
status: "接受预订",
tag: "FAN-CON · 热门抢购"
},
{
id: 6,
category: "fanmeeting",
title: "2026 SUNWOO 粉丝见面会《UNCHAINED》",
venue: "MYUNGHWA LIVE HALL (明和 Live Hall)",
priceKRW: "全场统一 99,000 韩元",
priceRMB: "~ ¥522 RMB",
krPresale: "2026.10.21 (周三) 8:00 PM (KST)",
globalPresale: "同步公售通道",
status: "少量名额",
tag: "个人FM · 近距离交互"
},
{
id: 7,
category: "fanmeeting",
title: "2026 CLOSE YOUR EYES FANCON",
venue: "Coex Artium WOORI BANK Hall",
priceKRW: "VIP 121,000 / R席 99,000 韩元",
priceRMB: "~ ¥638 / ¥522 RMB",
krPresale: "2026.10.20 (周二) 7:00 PM (KST)",
globalPresale: "无 Global 通道",
status: "NOL World 平台",
tag: "Weverse会员优先"

},
{
id: 8,
category: "dome",
title: "NMIXX 1ST WORLD TOUR FINALE IN INCHEON",
venue: "Inspire Arena (仁川 Inspire 竞技场)",
priceKRW: "指定座 154,000 韩元",
priceRMB: "~ ¥812 RMB",
krPresale: "2026.10.26 (周一) 8:00 PM (KST)",
globalPresale: "无提前预售",
status: "世巡终点站",
tag: "Inspire Arena · 大场馆"
},
{
id: 9,
category: "fanmeeting",
title: "2026 CHANYEOL B-day PARTY [B-side]",
venue: "YES24 LIVE HALL (首尔)",
priceKRW: "全席统一 77,000 韩元",
priceRMB: "~ ¥406 RMB",
krPresale: "2026.10.26 (周一) 8:00 PM (KST)",
globalPresale: "YES24 Global 通道",
status: "YES24独占",
tag: "生日Party · 限量席位"
}
];
let currentCategory = 'all';
// Simple i18n for dynamically rendered concert cards
const CARD_I18N = {
 bookBtn: { zh: '预订代抢通道', en: 'Book Presale', ko: '예매 대행 신청', ja: '代行予約' },
 krPresale: { zh: '韩国本土预售', en: 'KR Local Presale', ko: '한국 현지 선예매', ja: '韓国本土優先販売' },
 globalPresale: { zh: '全球 Global 预售', en: 'Global Presale', ko: '글로벌 예매', ja: 'Global 販売' }
};
// Weekday + common price/status phrase maps for card text
const WEEKDAY_MAP = {
 zh: { '周一':'周一','周二':'周二','周三':'周三','周四':'周四','周五':'周五','周六':'周六','周日':'周日' },
 en: { '周一':'Mon','周二':'Tue','周三':'Wed','周四':'Thu','周五':'Fri','周六':'Sat','周日':'Sun' },
 ko: { '周一':'월','周二':'화','周三':'수','周四':'목','周五':'금','周六':'토','周日':'일' },
 ja: { '周一':'月','周二':'火','周三':'水','周四':'木','周五':'金','周六':'土','周日':'日' }
};
const STATUS_MAP = {
 'YES24独占 · 预订中': { zh:'YES24独占 · 预订中', en:'YES24 Exclusive · Booking', ko:'YES24 독점 · 예약중', ja:'YES24独占 · 予約中' },
 '火热预订中': { zh:'火热预订中', en:'Hot Booking', ko:'인기 예약중', ja:'人気予約中' },
 '热抢中': { zh:'热抢中', en:'High Demand', ko:'열기 예약중', ja:'争奪中' },
 '本土独占': { zh:'本土独占', en:'Local Only', ko:'현지 독점', ja:'本土独占' },
 '接受预订': { zh:'接受预订', en:'Open for Booking', ko:'예약 접수중', ja:'予約受付中' },
 '少量名额': { zh:'少量名额', en:'Limited Slots', ko:'소량 명액', ja:'少数枠' },
 'NOL World 平台': { zh:'NOL World 平台', en:'NOL World Platform', ko:'NOL World 플랫폼', ja:'NOL World プラットフォーム' },
 '世巡终点站': { zh:'世巡终点站', en:'World Tour Finale', ko:'월드투어 피날레', ja:'ワールドツアー最終' },
 'YES24独占': { zh:'YES24独占', en:'YES24 Exclusive', ko:'YES24 독점', ja:'YES24独占' }
};
const PRICE_REPLACE = {
 en: [['全席统一','All seats'],['全场统一','All seats'],['指定席','Assigned'],['指定座','Assigned'],['VIP席','VIP'],['一般席','General'],['R席','R'],['韩元','KRW']],
 ko: [['全席统一','전석 통일'],['全场统一','전석 통일'],['指定席','지정석'],['指定座','지정석'],['VIP席','VIP'],['一般席','일반석'],['R席','R석'],['韩元','원']],
 ja: [['全席统一','全席統一'],['全场统一','全席統一'],['指定席','指定席'],['指定座','指定席'],['VIP席','VIP'],['一般席','一般席'],['R席','R席'],['韩元','ウォン']]
};
const TAG_REPLACE = {
 en: [['生日Party','Birthday Party'],['粉丝见面会','Fan Meeting'],['席位紧缺','Limited seats'],['顶级热度','Top demand'],['热门抢购','Hot sale'],['近距离交互','Close interaction'],['Weverse会员优先','Weverse member priority'],['高尺巨蛋','Gocheok Dome'],['个人FM','Solo FM']],
 ko: [['生日Party','생일 파티'],['粉丝见面会','팬미팅'],['席位紧缺','좌석 부족'],['顶级热度','최고 인기'],['热门抢购','인기 판매'],['近距离交互','근거리 소통'],['Weverse会员优先','Weverse 회원 우선'],['高尺巨蛋','고척돔'],['个人FM','개인 FM']],
 ja: [['生日Party','誕生日Party'],['粉丝见面会','ファンミーティング'],['席位紧缺','席不足'],['顶级热度','最高人気'],['热门抢购','人気販売'],['近距离交互','近距離交流'],['Weverse会员优先','Weverse会員優先'],['高尺巨蛋','高尺ドーム'],['个人FM','個人FM']]
};
const VENUE_REPLACE = {
 en: [['首尔','Seoul'],['首尔高尺巨蛋','Seoul Gocheok Dome'],['华正体育馆','Hwajeong Gym'],['仁川','Incheon'],['高丽大学华正体育馆','Korea Univ. Hwajeong'],['明和 Live Hall','Myunghwa Live Hall']],
 ko: [['首尔','서울'],['首尔高尺巨蛋','서울 고척돔'],['华正体育馆','화정체육관'],['仁川','인천'],['高丽大学华正体育馆','고려대 화정'],['明和 Live Hall','명화 라이브홀']],
 ja: [['首尔','ソウル'],['首尔高尺巨蛋','ソウル高尺ドーム'],['华正体育馆','華正体育館'],['仁川','仁川'],['高丽大学华正体育馆','高麗大華正'],['明和 Live Hall','明和ライブホール']]
};
function localizeCardText(text, type) {
 if (!text || iyLanguage === 'zh') return text;
 let out = text;
 if (type === 'date') {
   const map = WEEKDAY_MAP[iyLanguage] || {};
   Object.keys(map).forEach(k => { out = out.replace(k, map[k]); });
   // common global-only phrases
   const datePhrases = {
     en: [['无 Global 通道 (仅本土独占)','No Global (KR local only)'],['无 Global 通道','No Global channel'],['同步公售通道','Public sale (synced)'],['无提前预售','No early presale'],['YES24 Global 通道','YES24 Global']],
     ko: [['无 Global 通道 (仅本土独占)','글로벌 없음 (현지 전용)'],['无 Global 通道','글로벌 채널 없음'],['同步公售通道','공매 동기화'],['无提前预售','사전 예매 없음'],['YES24 Global 通道','YES24 Global']],
     ja: [['无 Global 通道 (仅本土独占)','Globalなし（本土のみ）'],['无 Global 通道','Globalなし'],['同步公售通道','一般販売同期'],['无提前预售','事前販売なし'],['YES24 Global 通道','YES24 Global']]
   };
   (datePhrases[iyLanguage] || []).forEach(([a,b]) => { out = out.split(a).join(b); });
   return out;
 }
 if (type === 'status') {
   return (STATUS_MAP[text] && STATUS_MAP[text][iyLanguage]) || text;
 }
 if (type === 'price') {
   const pairs = PRICE_REPLACE[iyLanguage] || [];
   pairs.forEach(([a,b]) => { out = out.split(a).join(b); });
   return out;
 }
 if (type === 'tag') {
   const pairs = TAG_REPLACE[iyLanguage] || [];
   pairs.forEach(([a,b]) => { out = out.split(a).join(b); });
   return out;
 }
 if (type === 'venue') {
   const pairs = VENUE_REPLACE[iyLanguage] || [];
   pairs.forEach(([a,b]) => { out = out.split(a).join(b); });
   return out;
 }
 return out;

}
// Modal select option texts
const OPT_I18N = {
 tierVip: ["VIP 席位 / 内场前排", "VIP / Front Floor", "VIP / 내장 전열", "VIP / 内場前列"],
 tierGeneral: ["指定席 / 一般看台", "Assigned / General", "지정석 / 일반", "指定席 / 一般"],
 tierAny: ["任意可接受席位", "Any available seat", "가능한 좌석 모두", "空席どちらでも"],
 qty1: ["1 张", "1 ticket", "1매", "1枚"],
 qty2: ["2 张", "2 tickets", "2매", "2枚"],
 planSuccess: ["成功后付款（需客服确认接单）", "Pay after success (confirm with support)", "성공 후 결제 (상담 확인 필요)", "成功後払い（要確認）"],
 planVip: ["优先服务咨询（需客服确认接单）", "Priority service (confirm with support)", "우선 서비스 상담 (확인 필요)", "優先サービス（要確認）"],
 tierBasic: ["基础档: 10% 服务费 (一般席位/看台)", "Basic: 10% fee (general seats)", "기본: 10% 수수료 (일반석)", "基本: 手数料10%（一般席）"],
 tierStd: ["标准档: 15% 服务费 (热门推荐)", "Standard: 15% fee (recommended)", "표준: 15% 수수료 (추천)", "標準: 手数料15%（おすすめ）"],
 tierRush: ["冲刺档: 20% 服务费 (稀缺前排 VIP)", "Rush: 20% fee (scarce VIP front)", "스프린트: 20% 수수료 (VIP 전열)", "スプリント: 手数料20%（希少VIP）"]
};
const M4_ENDPOINT = '';
const M4_TEST_MODE = new URLSearchParams(location.search).get('test') === '1';
// ===== 腾讯问卷链接 =====
// 去 https://wj.qq.com 创建问卷后，把问卷链接填到这里
// 问卷里建议设置以下题目（访客从主站带过去，也可直接在问卷里手填）：
//   1. 预约编号  2. 演出项目  3. 席位偏好  4. 张数  5. 服务方案  6. 昵称  7. 联系方式  8. 票面金额  9. 服务费  10. 总计
const TENCENT_SURVEY_URL = 'https://wj.qq.com/s2/28562942/nuw4/';
// ===== JSONBin 云端同步配置 =====
const JSONBIN_API_KEY = '$2a$10$dZ3XYEuTW9ITIfuXZXDzk.MJohX8ao0OT4y6CNs6uYyrl/kgzjpUi';
const JSONBIN_BIN_ID = '6aec7ba0ffd5d16053a8cd6a';
const JSONBIN_BASE_URL = 'https://api.jsonbin.io/v3/b/' + JSONBIN_BIN_ID;
// 推送单条预约到云端（先读后写合并，避免覆盖）
async function pushOrderToCloud(order) {
try {
// 读取云端现有数据
const res = await fetch(JSONBIN_BASE_URL + '/latest', {
method: 'GET',
headers: { 'X-Master-Key': JSONBIN_API_KEY }
});
let cloudOrders = [];
if (res.ok) {
const data = await res.json();
cloudOrders = (data.record && data.record.orders) || [];
}
// 追加新订单（按 id 去重）
const existIdx = cloudOrders.findIndex(o => o.id === order.id);
if (existIdx >= 0) {
cloudOrders[existIdx] = order; // 更新已有
} else {
cloudOrders.push(order);
}
// 写回云端
await fetch(JSONBIN_BASE_URL, {
method: 'PUT',
headers: {
'Content-Type': 'application/json',
'X-Master-Key': JSONBIN_API_KEY
},
body: JSON.stringify({ orders: cloudOrders })
});
return true;
} catch(err) {
console.warn('JSONBin push failed:', err);
return false;
}
}
// 腾讯问卷手动录入题目顺序（共15道，全部单行文本题）：
// q1.预约编号 q2.演出项目 q3.席位偏好 q4.张数 q5.服务方案 q6.昵称 q7.联系方式
// q8.票面金额（人民币） q9.服务费 q10.预估总计 q11.定金 q12.余款 q13.服务费率 q14.提交语言 q15.是否测试订单
function buildSurveyUrl(orderData) {
if (!TENCENT_SURVEY_URL) return null;
const params = new URLSearchParams({
q1: orderData.id,
q2: orderData.show,
q3: orderData.tier,
q4: orderData.qty,
q5: orderData.plan,
q6: orderData.nick,
q7: orderData.contact,
q8: orderData.faceTotal,
q9: orderData.fee,
q10: orderData.total,
q11: orderData.deposit,
q12: orderData.balance,
q13: orderData.rate ? (Math.round(orderData.rate * 100) + '%') : '',
q14: orderData.lang,
q15: orderData.testMode ? '是' : '否'
});
const sep = TENCENT_SURVEY_URL.includes('?') ? '&' : '?';
return TENCENT_SURVEY_URL + sep + params.toString();
}
async function sendM4Event(payload) {
if (!M4_ENDPOINT) return false;
try {
await fetch(M4_ENDPOINT, {
method: 'POST',
mode: 'no-cors',
headers: {'Content-Type': 'text/plain;charset=utf-8'},
body: JSON.stringify(payload),
keepalive: true
});
return true;
} catch (err) {
console.warn('Analytics request failed', err);
return false;
}
}
let userOrders = JSON.parse(localStorage.getItem('iykyk_m4_orders') || '[]');
const m4Group = sessionStorage.getItem('iykyk_m4_group') || ['A','B','C'][Math.floor(Math.random()*3)];
sessionStorage.setItem('iykyk_m4_group', m4Group);
const m4Rate = {A:0.10, B:0.15, C:0.20}[m4Group];
const m4Visitor = sessionStorage.getItem('iykyk_m4_visitor') || (crypto.randomUUID ? crypto.randomUUID() : String(Date.now()) + Math.random());
sessionStorage.setItem('iykyk_m4_visitor', m4Visitor);
function logM4(event, extra={}) {
const rows = JSON.parse(localStorage.getItem('iykyk_m4_events') || '[]');
rows.push({time: new Date().toISOString(), visitor: m4Visitor, group: m4Group, rate: m4Rate, event, ...extra});
localStorage.setItem('iykyk_m4_events', JSON.stringify(rows));
sendM4Event(rows[rows.length-1]);
}
if(!sessionStorage.getItem('iykyk_m4_viewed')) {
logM4('page_view');
sessionStorage.setItem('iykyk_m4_viewed', '1');
}
function renderConcerts(data) {
const container = document.getElementById('concert-grid');
container.innerHTML = '';
if(data.length === 0) {
container.innerHTML = `
<div class="col-span-full text-center py-12 text-ktext-light text-xs font-medium">
未搜寻到匹配的演出，可联系客服添加代抢需求。
</div>
`;
return;
}
data.forEach(item => {
const card = document.createElement('div');
card.className = "k-glass rounded-3xl p-6 shadow-card hover:shadow-soft transition-all duration-300 border border-kpink-200/80 flex flex-col justify-between space-y-4 group";
// Escape single quotes so titles containing ' (e.g. NCT WISH) do not break the onclick attribute
const safeTitle = item.title.replace(/'/g, "\\'");
card.innerHTML = `
<div class="space-y-3">
<div class="flex items-center justify-between gap-2">
<span class="text-[10px] font-bold px-3 py-1 rounded-full bg-kpink-100 text-kpink-600 border border-kpink-200">
${localizeCardText(item.tag, 'tag')}
</span>
<span class="text-[11px] font-semibold text-emerald-600 bg-emerald-50 px-2.5 py-0.5 rounded-full flex items-center gap-1">
<span class="w-1.5 h-1.5 rounded-full bg-emerald-500"></span> ${localizeCardText(item.status, 'status')}
</span>
</div>
<h3 class="font-extrabold text-base text-ktext-primary group-hover:text-kpink-600 transition-colors leading-snug">
${item.title}
</h3>
<div class="text-xs text-ktext-secondary space-y-1.5 pt-1">
<div class="flex items-center gap-2">
<i data-lucide="map-pin" class="w-3.5 h-3.5 text-kpink-400 shrink-0"></i>
<span>${localizeCardText(item.venue, 'venue')}</span>
</div>
<div class="flex items-center gap-2">
<i data-lucide="ticket" class="w-3.5 h-3.5 text-kpink-400 shrink-0"></i>
<span class="font-semibold text-ktext-primary">${localizeCardText(item.priceKRW, 'price')}</span>
<span class="text-ktext-light">(${item.priceRMB})</span>
</div>
</div>
<div class="bg-white/90 rounded-2xl p-3 border border-kpink-100 text-[11px] space-y-1.5 mt-3">
<div class="flex items-center justify-between font-semibold">
<span class="text-kpink-600 flex items-center gap-1">
<i data-lucide="zap" class="w-3 h-3"></i> ${CARD_I18N.krPresale[iyLanguage] || CARD_I18N.krPresale.zh}:
</span>
<span class="text-ktext-primary font-bold">${localizeCardText(item.krPresale, 'date')}</span>
</div>
<div class="flex items-center justify-between text-ktext-light">
<span>${CARD_I18N.globalPresale[iyLanguage] || CARD_I18N.globalPresale.zh}:</span>
<span>${localizeCardText(item.globalPresale, 'date')}</span>
</div>
</div>

</div>
<button onclick="openBookingForShow('${safeTitle}')" class="w-full mt-2 bg-gradient-to-r from-kpink-400 to-kpink-500 hover:from-kpink-500 hover:to-kpink-600 text-white font-bold py-2.5 rounded-full text-xs shadow-soft transition-all flex items-center justify-center gap-1.5">
<span>${CARD_I18N.bookBtn[iyLanguage] || CARD_I18N.bookBtn.zh}</span>
<i data-lucide="chevron-right" class="w-3.5 h-3.5"></i>
</button>
`;
container.appendChild(card);
});
if (window.lucide) lucide.createIcons();
}
function filterConcerts() {
const query = document.getElementById('concert-search').value.toLowerCase().trim();
let filtered = concertData;
if(currentCategory !== 'all') {
filtered = filtered.filter(item => item.category === currentCategory);
}
if(query) {
filtered = filtered.filter(item =>
item.title.toLowerCase().includes(query) ||
item.venue.toLowerCase().includes(query)
);
}
renderConcerts(filtered);
}
function setCategoryFilter(category) {
currentCategory = category;
document.querySelectorAll('.concert-tab').forEach(btn => {
btn.className = "concert-tab text-ktext-secondary hover:text-ktext-primary px-3.5 py-1 rounded-full transition-all";
});
const activeBtn = document.getElementById(`tab-${category}`);
if(activeBtn) {
activeBtn.className = "concert-tab bg-kpink-400 text-white px-3.5 py-1 rounded-full transition-all shadow-sm";
}
filterConcerts();
}
function updateCalculator() {
const showSelect = document.getElementById('calc-show');
const krwPrice = parseFloat(showSelect.value);
const markupRate = parseFloat(document.getElementById('calc-markup').value);
const rmbTicket = Math.round(krwPrice * 0.00527);
const serviceFeeRmb = Math.round(rmbTicket * markupRate);
const totalIykyk = rmbTicket + serviceFeeRmb;
document.getElementById('calc-cost-face').innerText = `¥ ${rmbTicket}`;
document.getElementById('calc-cost-iykyk').innerText = `¥ ${totalIykyk}`;
const feeDetailMap = {
 zh: `含服务费 ¥${serviceFeeRmb}`,
 en: `Incl. fee ¥${serviceFeeRmb}`,
 ko: `수수료 포함 ¥${serviceFeeRmb}`,
 ja: `手数料込 ¥${serviceFeeRmb}`
};
document.getElementById('calc-fee-detail').innerText = feeDetailMap[iyLanguage] || feeDetailMap.zh;
document.getElementById('calc-cost-scalper').innerText = `¥ ${Math.round(rmbTicket*2)} ~ ${Math.round(rmbTicket*3)}`;
}
function openBookingModal(planType) {
if(planType) {
document.getElementById('dw-plan').value = planType;
}
updateModalPrice();
logM4('quote_view',{show:document.getElementById('dw-show').value});
const modal = document.getElementById('booking-modal');
const card = document.getElementById('modal-card');
modal.classList.remove('opacity-0', 'pointer-events-none');
card.classList.remove('scale-95');
card.classList.add('scale-100');
}
function openBookingForShow(title) {
const selectEl = document.getElementById('dw-show');
for(let i=0; i<selectEl.options.length; i++) {
if(selectEl.options[i].value.includes(title.substring(0, 8))) {
selectEl.selectedIndex = i;
break;
}
}
openBookingModal();
}
function closeBookingModal() {
const modal = document.getElementById('booking-modal');
const card = document.getElementById('modal-card');
card.classList.remove('scale-100');
card.classList.add('scale-95');
modal.classList.add('opacity-0', 'pointer-events-none');
}
function updateModalPrice() {
const showSelect = document.getElementById('dw-show');
const selectedOpt = showSelect.options[showSelect.selectedIndex];
// 根据席位档位取对应票价：VIP 取 data-price-vip，一般席取 data-price-general，任意席按一般席估算
const tierVal = document.getElementById('dw-tier').value || '';
const isVip = tierVal.indexOf('VIP') !== -1;
const priceAttr = isVip ? 'data-price-vip' : 'data-price-general';
let krw = parseFloat(selectedOpt.getAttribute(priceAttr) || selectedOpt.getAttribute('data-price') || "77000");
const rmb = Math.round(krw * 0.00527);
const qty = Number(document.getElementById('dw-qty').value || 1);
const faceTotal = rmb * qty;
const fee = Math.round(faceTotal * m4Rate);
const total = faceTotal + fee;
const deposit = 100;
const balance = Math.max(0, total - deposit);
const tierTagMap = {
 zh: isVip ? 'VIP席' : '一般席',
 en: isVip ? 'VIP' : 'General',
 ko: isVip ? 'VIP석' : '일반석',
 ja: isVip ? 'VIP席' : '一般席'
};
const faceStr = {
 zh: `¥ ${faceTotal}（${qty} 张 · ${tierTagMap.zh} ${krw.toLocaleString()}韩元）`,
 en: `¥ ${faceTotal} (${qty} ticket${qty>1?'s':''} · ${tierTagMap.en} ${krw.toLocaleString()} KRW)`,
 ko: `¥ ${faceTotal}（${qty}매 · ${tierTagMap.ko} ${krw.toLocaleString()}원）`,
 ja: `¥ ${faceTotal}（${qty}枚 · ${tierTagMap.ja} ${krw.toLocaleString()}ウォン）`
};
document.getElementById('dw-face-val').innerText = faceStr[iyLanguage] || faceStr.zh;

const feeStr = {
 zh: `服务费 ¥${fee} (${Math.round(m4Rate*100)}%) · 总计 ¥${total} · 定金 ¥${deposit}（抵扣总价）· 余款 ¥${balance}`,
 en: `Fee ¥${fee} (${Math.round(m4Rate*100)}%) · Total ¥${total} · Deposit ¥${deposit} (deductible) · Balance ¥${balance}`,
 ko: `수수료 ¥${fee} (${Math.round(m4Rate*100)}%) · 합계 ¥${total} · 예약금 ¥${deposit} · 잔액 ¥${balance}`,
 ja: `手数料 ¥${fee} (${Math.round(m4Rate*100)}%) · 合計 ¥${total} · 預り金 ¥${deposit} · 残額 ¥${balance}`
};
document.getElementById('dw-deposit-val').innerText = feeStr[iyLanguage] || feeStr.zh;
}
function submitBooking(e) {
e.preventDefault();
const showSelect = document.getElementById('dw-show');
const showName = showSelect.value;
const selectedOpt = showSelect.options[showSelect.selectedIndex];
const tier = document.getElementById('dw-tier').value;
const isVip = tier.indexOf('VIP') !== -1;
const krw = parseFloat(selectedOpt.getAttribute(isVip ? 'data-price-vip' : 'data-price-general') || selectedOpt.getAttribute('data-price') || "77000");
const qty = document.getElementById('dw-qty').value;
const plan = document.getElementById('dw-plan').value;
const nick = document.getElementById('dw-name').value.trim() || '（未填写）';
const contact = document.getElementById('dw-contact').value.trim() || '（未填写）';
const newOrderId = 'M4-' + Date.now().toString(36).toUpperCase() + '-' + Math.random().toString(36).slice(2,6).toUpperCase();
const rmbUnit = Math.round(krw * 0.00527);
const qtyNum = Number(qty || 1);
const faceTotal = rmbUnit * qtyNum;
const fee = Math.round(faceTotal * m4Rate);
const total = faceTotal + fee;
const statusMap = {
 zh: '预约申请已保存 · 待联系客服确认（非已付款订单）',
 en: 'Request saved · Contact support to confirm (not paid yet)',
 ko: '신청 저장됨 · 상담 확인 대기 (미결제)',
 ja: '申請保存済 · サポート確認待ち（未払い）'
};
const adminStatus = '待确认';
userOrders.push({
id: newOrderId,
show: showName,
qty: qtyNum,
tier: tier,
plan: plan,
nick: nick,
contact: contact,
krw: krw,
faceTotal: faceTotal,
fee: fee,
total: total,
deposit: 100,
balance: Math.max(0, total - 100),
rate: m4Rate,
status: statusMap[iyLanguage] || statusMap.zh,
adminStatus: adminStatus,
lang: iyLanguage,
testMode: M4_TEST_MODE,
createdAt: new Date().toISOString(),
updatedAt: new Date().toISOString()
});
localStorage.setItem('iykyk_m4_orders', JSON.stringify(userOrders));
logM4('booking_request', {show: showName, qty, tier, request_id: newOrderId, test_mode: M4_TEST_MODE});
closeBookingModal();
document.getElementById('search-order-input').value = newOrderId;
searchOrder();
scrollToSection('orders');
document.getElementById('after-booking-id').textContent = newOrderId;
document.getElementById('payment-unlock').checked = false;
togglePayment();
document.getElementById('m4-storage-note').textContent = ' 预约已提交，团队后台将自动收到你的预约信息。';
const afterModal = document.getElementById('after-booking-modal');
afterModal.classList.remove('hidden');
afterModal.classList.add('flex');
const toastMap = {
 zh: '预约申请已保存，请添加客服确认',
 en: 'Request saved — please add support on WeChat',
 ko: '신청 저장됨 · 위챗 상담을 추가하세요',
 ja: '申請を保存しました。サポートを追加してください'
};
showToast(toastMap[iyLanguage] || toastMap.zh);
// ===== 推送到 JSONBin 云端（让 admin 后台能看到所有人预约） =====
const lastOrderForCloud = userOrders[userOrders.length - 1];
pushOrderToCloud(lastOrderForCloud);
}
function togglePayment() {
const checkbox = document.getElementById('payment-unlock');
if(M4_TEST_MODE) {
checkbox.checked = false;
showToast('测试模式禁止展示付款码');
}
document.getElementById('payment-options').classList.toggle('hidden', !checkbox.checked || M4_TEST_MODE);
if(checkbox.checked && !M4_TEST_MODE) logM4('payment_information_unlocked');
}
function recordWechatClick() {
logM4('wechat_intent_click', {test_mode: M4_TEST_MODE});
showToast('已记录客服意向；请自行在微信添加客服 Chloe_ii0514');
}
function closeAfterBooking() {
const el = document.getElementById('after-booking-modal');
el.classList.add('hidden');
el.classList.remove('flex');
}
function copyBookingId() {
const id = document.getElementById('after-booking-id').textContent;
navigator.clipboard?.writeText(id).then(() => showToast('预约编号已复制'));
}
function searchOrder() {
const query = document.getElementById('search-order-input').value.trim();
const box = document.getElementById('order-result-box');
if (!query) {
showToast('请输入订单编号');
return;
}
const found = userOrders.find(o => o.id === query || query.toUpperCase() === 'IY-2026-8812');
if(!found && query.toUpperCase() !== 'IY-2026-8812') {
box.classList.add('hidden');
showToast('未找到本浏览器保存的预约编号');
return;
}
if (found) {
document.getElementById('res-order-id').innerText = '#' + found.id;
document.getElementById('res-show-title').innerText = found.show;
document.getElementById('res-status-badge').innerText = found.status;
} else {
document.getElementById('res-order-id').innerText = '#IY-2026-8812';
document.getElementById('res-show-title').innerText = '2026 CHENLE B-day PARTY [Lele’s Show 2]';
const badgeMap = {
 zh: 'YES24 本土实名账号锁定中',
 en: 'YES24 local verified account locking',
 ko: 'YES24 현지 실명 계정 잠금 중',
 ja: 'YES24 本土実名アカウント確保中'
};
document.getElementById('res-status-badge').innerText = badgeMap[iyLanguage] || badgeMap.zh;
}
box.classList.remove('hidden');
}
function scrollToSection(id) {
const el = document.getElementById(id);
if(el) {
el.scrollIntoView({ behavior: 'smooth', block: 'start' });
}
}

function showToast(msg) {
const toast = document.getElementById('toast');
document.getElementById('toast-message').innerText = msg;
toast.classList.remove('opacity-0', 'pointer-events-none');
setTimeout(() => {
toast.classList.add('opacity-0', 'pointer-events-none');
}, 3200);
}
// Lightweight Multi-Language Localization Engine
const IY_LANGS = {
"navServices": ["服务优势", "Services", "서비스 장점", "特长"],
"navConcerts": ["演出 Schedule", "Concerts", "공연 일정", "公演日程"],
"navCalc": ["试算测算", "Calculator", "요금 계산", "料金計算"],
"navOrders": ["订单查询", "Orders", "주문 조회", "注文照会"],
"navTrust": ["安全保障", "Trust & Safety", "안전 보장", "安全保障"],
"btnSearch": ["查询订单", "Search Order", "주문 검색", "注文検索"],
"btnBook": ["立即预订", "Book Now", "지금 예약", "今すぐ予約"],
"noticeTitle": ["限量预约服务", "Limited Booking Service", "한정 예약 서비스", "数量限定予約"],
"noticeBody": ["：目前仅接受少量购票协助申请。提交预约后请添加微信客服 Chloe_ii0514 确认是否接单、最终报价及退款条款；未经确认请勿付款。", " We currently accept limited booking assistance. After submitting, add WeChat Chloe_ii0514 to confirm capacity and final price.", " 현재 소수의 티켓 지원 신청만 받습니다. 신청 후 위챗 Chloe_ii0514로 접수 여부를 확인하세요.", " 现在、少数のチケット購入サポートのみ受け付けています。申請後WeChat Chloe_ii0514にご確認ください。"],
"heroBadge": ["IYKYK / 韩国本土预售优先抢订服务", "IYKYK / Korea Local Presale Concierge", "IYKYK / 한국 현지 선예매 대행", "IYKYK / 韓国本土優先予約サポート"],
"heroTitle1": ["直通韩国本土优先预售通道", "Direct Access to Korean Presales", "한국 현지 우선 예매 직통", "韓国本土優先販売ルート直行"],
"heroTitle2": ["安全·透明·极速抢占优质席位", "Safe · Transparent · Instant VIP Booking", "안전 · 투명 · 초고속 VIP 좌석 선점", "安全・透明・極速VIP席確保"],
"heroDesc": ["由专业团队提供韩国本土实名认证账号与优先开售抢订支持。绕过 Global 通道漫长等候与天价黄牛，采用“抢到后付服务费 / 未成功定金全退”安全保障机制。", "Powered by verified local Korean accounts. Skip global queues and scalper markups with our success-first security model.", "한국 현지 실명 인증 계정으로 빠른 예매를 지원합니다. 실패 시 100% 환불 보장.", "韓国本土実名認証アカウントで最速確保。失敗時全額返金保障。"],
"v1Title": ["成功后再付尾款", "Pay After Success", "성공 후 결제", "成功後払い"],
"v1Sub": ["第三方托管低风险", "Low risk handling", "낮은 리스크", "低リスク"],
"v2Title": ["本土提前优先购票", "Local Priority Access", "현지 우선 예매", "本土優先購入"],
"v2Sub": ["优先抢占内场与VIP", "VIP floor seat priority", "VIP 내장 석선점", "VIP席優先"],
"v3Title": ["在韩实名认证账号", "Verified KR Accounts", "한국 실명 계정", "韓国実名認証"],
"v3Sub": ["避开海外 IP 排队限制", "Bypass overseas IP limits", "해외 IP 제한 우회", "海外IP制限回避"],
"v4Title": ["费用明细公开透明", "Transparent Pricing", "투명한 수수료", "透明な料金"],
"v4Sub": ["服务费 10%-15% 起", "From 10%-15% service fee", "수수료 10%부터", "手数料10%〜"],
"statusLabel": ["当前本土预售通道运行中：", "Local presale channel active: ", "현재 선예매 채널 가동 중: ", "現在本土優先ルート稼働中："],
"statusSuffix": ["等演出接单中", "shows open for booking", "등 공연 예약 중", "などの公演受付中"],
"concertsHeader": ["热门演出与代抢预订列表", "Live Concerts & Presale Schedule", "인기 공연 및 예매 목록", "热门公演・予約リスト"],
"concertsSubHeader": ["同步韩国本土 (KR Page) 与全球 (Global Page) 官方预售节点", "Synchronized with official KR and Global ticketing release times", "한국 현지 및 글로벌 예매 일정 동기화", "韓国本土およびGlobal公式発売時間を同期"],
"searchPlaceholder": ["搜索艺人/场地...", "Search artist / venue...", "아티스트 / 공연장 검색...", "アーティスト・会場を検索..."],
"tabAll": ["全部", "All", "전체", "すべて"],
"tabDome": ["大型/Dome", "Dome / Arena", "돔 / 아레나", "ドーム・アリーナ"],
"tabFM": ["FM/Party", "Fan Meeting", "팬미팅", "ファンミ"],
"plansHeader": ["选择最适合您的代抢服务方案", "Select Your Service Plan", "맞춤형 서비스 플랜 선택", "サービスプランを選択"],
"plansSubHeader": ["包含本土实名认证账号使用权、抢订操作及全程票务对接指导", "Includes local account access, rapid booking execution, and end-to-end guidance", "현지 실명 계정 및 1:1 지원 포함", "本土実名認証アカウント利用・サポート付き"],
"planATitle": ["抢到后付模式 (Success-First)", "Success-First Plan", "성공 후 결제 플랜", "成功後払いプラン"],
"planADesc": ["资金安全优先，出票成功后再付主体服务费", "Security first: service fee paid after ticket confirmed", "티켓 확보 후 수수료 결제", "チケット確保後に手数料お支払い"],
"planBTitle": ["VIP 前排锁位方案 (VIP Priority)", "VIP Priority Plan", "VIP 우선 선점 플랜", "VIP優先確保プラン"],
"planBDesc": ["适合拟冲刺首尔内场 VIP / 极其紧缺席位", "Dedicated for high-demand Seoul floor VIP seats", "서울 VIP Floor 최우선 지원", "ソウルVIP席専用アタック"],
"calcHeader": ["代抢服务费用实时测算", "Live Service Fee Calculator", "실시간 서비스 요금 계산", "サービス料金リアルタイム計算"],
"calcSubHeader": ["拒绝黄牛动辄数倍的恶劣溢价。依据官方票面与合理服务费率计算，拒绝隐藏收费。", "No scalper markups. Clear calculation based on official face value and fixed rates.", "황돈 프리미엄 거부. 공식 티켓가 기준 투명 계산.", "高額転売価格を防止。公式チケット価格に基づく透明計算。"],
"calcSelectShow": ["选择拟代抢演出项目", "Select Concert", "공연 선택", "公演を選択"],
"calcSelectTier": ["服务档位", "Service Tier", "서비스 등급", "区分"],
"orderHeader": ["订单进度查询与状态跟踪", "Order Tracking Portal", "주문 진행 상황 조회", "注文状況照会"],
"orderSubHeader": ["输入订单号（如 M4-XXXX 或 IY-2026-8812）进行检索", "Enter your reference ID (e.g. M4-XXXX) to track real-time progress", "예약 번호(M4-XXXX)를 입력하세요", "予約番号（M4-XXXX）を入力してください"],
"orderSearchPlaceholder": ["输入订单号或手机/微信账号", "Enter reference ID or WeChat", "예약 번호 입력", "予約番号を入力"],
"trustHeader": ["服务保障与隐私承诺", "Safety & Guarantee Protocol", "안전 보장 및 개인정보 약속", "安全保障・プライバシー約束"],
"t1Title": ["严格个人信息保护", "Strict Data Privacy", "개인정보 엄격 보호", "個人情報厳重保護"],
"t1Desc": ["客户所有身份证照及观演人信息仅用于本次门票实名绑定与官方查验，抢票结束后即刻清空。", "Personal ID info is used only for official real-name verification and deleted immediately after.", "입장 확인용 정보는 예매 완료 후 즉시 파기됩니다.", "本人確認用データはチケット確保後即座に破棄されます。"],
"t2Title": ["真实本土合规账号", "Genuine KR Accounts", "합법 현지 계정 사용", "正規本土アカウント"],
"t2Desc": ["仅使用在韩留学生持有之本土实名认证账号，避免海外网络封锁，杜绝非法外挂脚本导致的封号风险。", "Verified accounts owned by local students in Korea. No risk of bot bans.", "한국 현지 실명 계정 사용으로 블락 위험 제로.", "韓国本土の正規認証済みアカウント使用。"],
"t3Title": ["未出票 100% 全额退款", "100% Refund Guarantee", "실패 시 100% 환불", "失敗時全額返金"],
"t3Desc": ["若因席位极度紧缺导致未能成功出票，所有定金无条件原路退回。", "If tickets cannot be secured, 100% of your deposit is refunded immediately.", "티켓 미확보 시 모든 예약금 즉시 원상 복구.", "チケットが確保できなかった場合、預かり金は全額返金。"],
"modalTitle": ["预订代抢服务", "Book Ticket Assistance", "티켓 예매 지원 신청", "代行予約"],
"f1": ["1. 选择演出项目", "1. Select Concert", "1. 공연 선택", "1. 公演を選択"],
"f2": ["2. 席位偏好", "2. Seat Preference", "2. 좌석 선호", "2. 座席希望"],
"f3": ["3. 张数", "3. Quantity", "3. 수량", "3. 枚数"],
"f4": ["4. 付费服务方案", "4. Service Plan", "4. 플랜 선택", "4. プラン"],
"f5": ["5. 昵称（请勿填写证件姓名）", "5. Nickname (No Legal ID)", "5. 닉네임", "5. ニックネーム"],
"f6": ["6. 联系方式（可选；请勿填写敏能信息）", "6. Contact (Optional)", "6. 연락처 (선택)", "6. 連絡先（任意）"],
"nickPlaceholder": ["如：K-pop fan", "e.g. K-pop fan", "예: K-pop fan", "例: K-pop fan"],
"contactPlaceholder": ["可留微信或邮箱；请勿提供敏感信息", "WeChat ID or Email", "위챗 또는 이메일", "WeChatまたはメール"],
"btnSubmitBooking": ["提交预约申请 · 联系客服确认", "Submit Request & Contact Service", "신청서 제출 및 상담", "予約代行を送信"],
"afterTitle": ["💗 预约申请已提交（待人工确认）", "💗 Booking Request Submitted", "💗 예약 신청 완료", "💗 予約申請完了"],
"afterRef": ["预约编号：", "Reference ID: ", "예약 번호: ", "予約番号："],
"copyBtn": ["复制", "Copy", "복사", "コピー"],
"step1Header": ["第一步：添加微信客服 Chloe_ii0514", "Step 1: Add WeChat Chloe_ii0514", "1단계: 위챗 Chloe_ii0514 추가", "ステップ1: WeChat Chloe_ii0514 を追加"],
"step1Text": ["请主动添加客服并发送预约编号、演唱会和场次，确认是否还有少量服务名额、票价、¥100 可抵扣定金、10%–20% 服务费、实名入场规则及退款条件。", "Send your reference ID and concert details to WeChat customer service to confirm availability.", "예약 번호와 공연 정보를 위챗으로 전송하여 접수 여부를 확인하세요.", "予約番号と公演情報をWeChatで送信して確定してください。"],
"copyWechat": ["复制微信号", "Copy WeChat ID", "위챗 ID 복사", "WeChat IDコピー"],
"intentBtn": ["我已复制微信号 · 记录客服意向", "I Copied WeChat ID", "위챗 ID 복사 완료", "WeChat ID コピー完了"],
"step2Header": ["第二步：客服确认后选择支付方式", "Step 2: Pay Only After Confirmation", "2단계: 확인 후 결제", "ステップ2: 確認後にお支払い"],
"checkLabel": ["我确认已与客服沟通，核实了接单能力、实名入场要求、最终报价及退款条款。", "I confirm I have verified capacity, ID rules, and terms with customer service.", "고객센터와 가격 및 조건 확인을 완료했습니다.", "スタッフと価格および条件を確認済みです。"],
"gotIt": ["我知道了", "Got It", "확인", "了解しました"],
"faceLabel": ["票面估算：", "Face value: ", "티켓 가격: ", "チケット価格："],
"feeLabel": ["服务费及费用明细：", "Service fee detail: ", "수수료 및 비용: ", "手数料・費用明細："],
"depositNote": ["* 定金 ¥100 可抵扣最终费用，并非额外收费；抢票失败全额退还定金。少量接单，实际票价、库存、服务费及付款时机以客服书面确认为准。请勿在客服确认前付款。", "* ¥100 deposit is deductible. Full refund if unsuccessful. Final price confirmed by support. Do not pay before confirmation.", "* 예약금 ¥100은 최종 비용에서 차감됩니다. 실패 시 전액 환불. 결제 전 고객센터 확인 필수.", "* 預かり金¥100は最終費用から差し引きます。失敗時全額返金。確認前に支払わないでください。"],
"modalWarning": ["⚠️ 限量人工接单：提交仅代表预约申请，不代表已接单、已付款或已购票。受邀朋友请使用 ?test=1 测试链接，不要付款。请核实实名制及官方售票平台规则。", "⚠️ Limited manual intake: submitting is only a request. Use ?test=1 for testing. Do not pay before confirmation.", "⚠️ 한정 수동 접수: 제출은 신청일 뿐입니다. 테스트는 ?test=1 사용. 확인 전 결제 금지.", "⚠️ 限定受付：提出は申請のみです。テストは?test=1。確認前に支払わないでください。"],
"planBookBtn": ["按此方案预订", "Book this plan", "이 플랜으로 예약", "このプランで予約"],
"depositLine": ["定金 ¥100", "Deposit ¥100", "예약금 ¥100", "預り金 ¥100"],
"depositLineSub": ["+ 服务费 10%–20%（定金抵扣最终费用）", "+ Service fee 10%–20% (deposit deductible)", "+ 수수료 10%–20% (예약금 차감)", "+ 手数料 10%–20%（預り金差し引き）"],
"planA1": ["分配专人韩国本土实名认证账号", "Dedicated verified local KR account", "전담 한국 실명 계정 배정", "専任の韓国本土実名アカウント"],
"planA2": ["抢票未成功：¥100 定金全额退还", "If unsuccessful: full ¥100 deposit refund", "실패 시 ¥100 예약금 전액 환불", "失敗時：¥100全額返金"],
"planA3": ["成功出票后支付剩余款项，已付 ¥100 定金抵扣最终应付金额", "Pay remaining after success; ¥100 deposit deducted", "성공 후 잔액 결제, ¥100 예약금 차감", "成功後に残額支払い、¥100は差し引き"],
"planB1": ["优先调配高响应度本土账号组", "Priority high-response local account pool", "고응답 현지 계정 우선 배정", "高応答本土アカウント優先"],
"planB2": ["专属客服一对一全程同步抢票截图", "1:1 support with live booking screenshots", "1:1 전담 상담 + 실시간 캡처", "専属サポートとリアルタイム画面共有"],
"planB3": ["未出票：¥100 定金全额退还", "No ticket: full ¥100 deposit refund", "미확보 시 ¥100 전액 환불", "未確保時：¥100全額返金"],
"calcFaceLabel": ["官方原票价 (折合RMB)", "Official face value (RMB)", "공식 티켓가 (RMB)", "公式チケット価格（RMB）"],
"calcRateNote": ["按实时汇率折算", "Converted at live rate", "실시간 환율 적용", "リアルタイム為替換算"],
"calcIykykLabel": ["IYKYK 预估总支出", "IYKYK estimated total", "IYKYK 예상 총비용", "IYKYK 見積総額"],
"calcScalperLabel": ["传统二手黄牛参考价", "Typical scalper price", "암표 참고가", "転売相場参考"],
"calcScalperNote": ["200%-300% 天价溢价", "200%–300% markup", "200%–300% 프리미엄", "200%〜300% 上乗せ"],
"btnQueryStatus": ["查询状态", "Check Status", "상태 조회", "状態確認"],
"step1Title": ["抢票需求提交与方案锁定", "Request submitted & plan locked", "신청 제출 및 플랜 확정", "申請提出・プラン確定"],
"step1Desc": ["客户信息提交成功，第三方退订担保生效", "Info submitted; refund guarantee active", "정보 제출 완료, 환불 보장 적용", "情報提出完了、返金保証適用"],

"step2Title": ["本土实名认证账号完成匹配", "Local verified account matched", "현지 실명 계정 매칭 완료", "本土実名アカウント割当完了"],
"step2Desc": ["已分发首尔本土高响应 YES24 账号", "Seoul high-response YES24 account assigned", "서울 고응답 YES24 계정 배정", "ソウル高応答YES24アカウント割当"],
"step3Title": ["等待韩国本土预售窗口开启", "Waiting for KR local presale window", "한국 현지 선예매 오픈 대기", "韓国本土優先販売開始待ち"],
"step3Desc": ["抢票人员已准备完毕，预计开售即刻进入抢订", "Team ready; will enter queue at open", "예매팀 준비 완료, 오픈 즉시 진입", "スタッフ準備完了、開始と同時に確保"],
"step4Title": ["出票凭证确认与尾款结算", "Ticket proof & final payment", "티켓 확인 및 잔금 결제", "チケット確認と残金精算"],
"step4Desc": ["发送官方订票截图与实体/电子票查验", "Official booking proof & e-ticket check", "공식 예매 캡처 및 티켓 확인", "公式予約画面とチケット確認"],
"payWarning": ["付款前请注意：当前仅接受少量购票协助申请。预约并不保证抢票成功。请先通过微信客服确认接单、最终费用、付款条件及退款规则，未经客服确认请勿转账。请核实收款方名称与客服提供的信息一致。本站不会自动验证付款，付款后需由客服人工核实。", "Before payment: limited capacity only. Booking does not guarantee success. Confirm with WeChat support first — do not transfer before confirmation. Verify the recipient name. Site does not auto-verify payments.", "결제 전 주의: 소량만 접수. 성공을 보장하지 않습니다. 위챗 상담 확인 후 결제하세요. 수취인 확인 필수.", "支払前注意：少数のみ受付。成功は保証されません。WeChat確認後に支払ってください。受取人名を確認。"],
"m4TestNote": ["📋 M4 测试说明：如果你是受邀体验流程的朋友，请使用网址参数 ?test=1 进入测试模式。测试预约不代表真实购票需求，请勿付款。", "📋 M4 test: invited testers use ?test=1. Test bookings are not real — do not pay.", "📋 M4 테스트: ?test=1 로 테스트. 실제 결제는 하지 마세요.", "📋 M4テスト：?test=1 でテスト。実際の支払いはしないでください。"],
"payTip": ["提示：以上为扫码收款示例码，并非自动跳转的支付链接；请在付款前核实收款账户。无需向网站提交付款密码或证件照片。", "Note: sample QR codes only, not live payment links. Verify the account before paying. Never submit passwords or ID photos to the site.", "안내: 예시 QR이며 자동 결제 링크가 아닙니다. 결제 전 계좌를 확인하세요.", "注意：サンプルQRです。支払前に口座を確認。パスワードや身分証は送信しないでください。"],
"defaultBadge": ["YES24 本土实名账号锁定中", "YES24 local verified account locking", "YES24 현지 실명 계정 잠금 중", "YES24 本土実名アカウント確保中"],
"planABadge": ["限量预约 · 客服确认后付款", "Limited · Pay after support confirms", "한정 예약 · 상담 확인 후 결제", "限定予約 · 確認後支払い"]
};
const IY_CODES = ['zh', 'en', 'ko', 'ja'];
let iyLanguage = 'zh';
function applyLanguage() {
const idx = IY_CODES.indexOf(iyLanguage);
document.querySelectorAll('[data-i18n]').forEach(el => {
const key = el.dataset.i18n;
if(IY_LANGS[key] && IY_LANGS[key][idx]) {
el.innerText = IY_LANGS[key][idx];
}
});
document.querySelectorAll('[data-i18n-placeholder]').forEach(el => {
const key = el.dataset.i18nPlaceholder;
if(IY_LANGS[key] && IY_LANGS[key][idx]) {
el.placeholder = IY_LANGS[key][idx];
}
});
// Modal select options
document.querySelectorAll('[data-i18n-opt]').forEach(el => {
const key = el.dataset.i18nOpt;
if(OPT_I18N[key] && OPT_I18N[key][idx]) {
el.textContent = OPT_I18N[key][idx];
}
});
document.documentElement.lang = iyLanguage === 'zh' ? 'zh-CN' : iyLanguage;
}
function setSiteLanguage(code) {
if(!IY_CODES.includes(code)) return;
iyLanguage = code;
localStorage.setItem('iykyk_language', code);
applyLanguage();
// Re-render dynamic concert cards so language-aware labels update
filterConcerts();
// Refresh modal price text if modal is open / values present
if (document.getElementById('dw-show')) updateModalPrice();
// Refresh calculator fee detail text
if (document.getElementById('calc-show')) updateCalculator();
}
// ===== ADMIN LOGIN =====
const ADMIN_PASSWORD = 'iykyk2026';
function openAdminLogin() {
const modal = document.getElementById('admin-login-modal');
modal.classList.remove('hidden');
modal.classList.add('flex');
document.getElementById('admin-pwd-input').value = '';
document.getElementById('admin-pwd-error').classList.add('hidden');
setTimeout(() => document.getElementById('admin-pwd-input').focus(), 50);
}
function closeAdminLogin() {
const modal = document.getElementById('admin-login-modal');
modal.classList.add('hidden');
modal.classList.remove('flex');
}
function verifyAdmin() {
const input = document.getElementById('admin-pwd-input').value;
if (input === ADMIN_PASSWORD) {
sessionStorage.setItem('iykyk_admin_authed', '1');
closeAdminLogin();
window.location.href = 'admin.html';
} else {
document.getElementById('admin-pwd-error').classList.remove('hidden');
}
}
window.onload = function() {
if (window.lucide) lucide.createIcons();
const stored = localStorage.getItem('iykyk_language');
if (stored && IY_CODES.includes(stored)) {
iyLanguage = stored;
document.getElementById('language-picker').value = stored;
}
renderConcerts(concertData);
updateCalculator();
applyLanguage();
}
</script>
</body>
</html>
