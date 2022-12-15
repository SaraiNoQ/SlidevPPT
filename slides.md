---
# try also 'default' to start simple
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# show line numbers in code blocks
lineNumbers: true
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# persist drawings in exports and build
drawings:
  persist: false
# use UnoCSS
css: unocss
---

<h1 class="tracking-widest font-mono">工程实践3</h1>

<span class="font-sans tracking-wider text-lg font-serif">课程答辩2</span>

<div class="pt-12">
  <span @click="$slidev.nav.next" class="px-2 py-1 rounded cursor-pointer font-serif" hover="bg-white bg-opacity-10">
    开始<carbon:arrow-right class="inline-block pl-1"/>
  </span>
</div>

<div class="abs-br m-6 flex gap-2">
  <button @click="$slidev.nav.openInEditor()" title="Open in Editor" class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon:edit />
  </button>
  <a href="https://github.com/slidevjs/slidev" target="_blank" alt="GitHub"
    class="text-xl icon-btn opacity-50 !border-none !hover:text-white">
    <carbon-logo-github />
  </a>
</div>

---

# National standard for Software Testing

<span class="tracking-normal font-serif text-xl font-bold">软件测试依据的国家技术标准规范</span>

<!-- - <span class="text-xl font-semibold">软件工程标准</span> -->
- 📝 **信息系统及软件完整性级别** - <kbd>GB/T 17544-1998</kbd>
- 🎨 **软件质量模型与度量** - <kbd>GB/T 16260-2006</kbd>
- 🧑‍💻 **软件工程产品评价** - <kbd>GB/T 18905-2002</kbd>
- 🤹 **计算机软件文档编制规范** - <kbd>GB/T 8567-2006</kbd>
- 🎥 **计算机软件测试文件编制规范** - <kbd>GB/T 9386-2008</kbd>
- 📤 **软件质量要求与评价( SQuaRE )指南** - <kbd>GB/T 25000.1-2010</kbd>
- 🧩 **应用软件产品测试规范** - <kbd>CSTCJSBZ02</kbd>
- 🛠 **软件产品测试评分标准** - <kbd>CSTCJSBZ03</kbd>

<br>
<br>

<span class="font-serif">更多的国家标准请参考：[软件工程相关标准](https://www.cnblogs.com/Mr-Kenson/p/16050196.html)</span>

<!--
You can have `style` tag in markdown to override the style for the current page.
Learn more: https://sli.dev/guide/syntax#embedded-styles
-->

<style>
h1 {
  background-color: #2B90B6;
  background-image: linear-gradient(45deg, #4EC5D4 20%, #146b8c 30%);
  background-size: 100%;
  -webkit-background-clip: text;
  -moz-background-clip: text;
  -webkit-text-fill-color: transparent;
  -moz-text-fill-color: transparent;
}
li {
  font-family: "Baskerville",
    "Georgia",
    "Liberation Serif",
    "Kaiti SC",
    "STKaiti",
    "AR PL UKai CN",
    "AR PL UKai HK",
    "AR PL UKai TW",
    "AR PL UKai TW MBE",
    "AR PL KaitiM GB",
    "KaiTi",
    "KaiTi_GB2312",
    "DFKai-SB",
    "TW-Kai",
    "serif";
}
</style>

---

# Guidelines for My Project

<span class="tracking-normal font-serif text-xl font-bold">项目测试中遵循的测试标准和原则</span>

|     |     |
| --- | --- |
| <span class="fff">测试证明缺陷的存在</span> | <span class="fff">即使在测试过程中没有发现失效，也不能证明证明没有缺陷，即<strong>零缺陷是不可能的</strong>。</span> |
| <span class="fff">穷尽测试是不可能的</span> | <span class="fff"><strong>穷尽测试（输入和前提条件的所有组合）是不可行的</strong>，所以我们应利用风险分析、测试技术和优先级确定测试工作量。</span> |
| <span class="fff">测试的尽早介入可以节省时间和成本</span> | <span class="fff">测试的尽早介入有时也称为测试的左移，<strong>尽早开始测试可以减少项目时间和成本</strong>。</span> |
| <span class="fff">缺陷的群集效应</span> | <span class="fff"><strong>在BUG的周围往往会发现更多的问题</strong>，所以这些应该作为风险分析的重要输入。</span> |
| <span class="fff">杀虫剂悖论</span> | <span class="fff">就像杀虫剂在一段时间后对杀死昆虫不再有效一样，如果多次重复同样的测试，最终这些测试将不再能够发现任何新的缺陷，所以我们应经常检查测试用例并且生成新的测试用例。</span> |
| <span class="fff">测试活动依赖于测试周境</span> | <span class="fff"><strong>测试在不同周境下是不同的</strong>。所以不应该以完全相同的方法去测试两个不同的系统。</span> |
| <span class="fff">不存在缺陷的谬论</span> | <span class="fff">软件测试不仅仅是为了找出BUG而存在的活动，而是还需要确认软件是否满足用户的期望和需求，<strong>如果产品不能满足用户的需求，即使没有出现任何缺陷，这个产品也是失败的</strong></span> |

<!-- <arrow v-click="1" x1="280" y1="250" x2="170" y2="172" color="#564" width="3" arrowSize="1" />
<arrow v-click="2" x1="280" y1="350" x2="170" y2="272" color="#564" width="3" arrowSize="1" />
<p v-after class="absolute bottom-23 left-45 opacity-30 transform -rotate-10">Here!</p> -->

<style>
.fff {
  font-size: 14px;
  line-height: 16px !important;
  font-family: 
    "Georgia",
    "Nimbus Roman No9 L",
    "Songti SC",
    "Noto Serif CJK SC",
    "Source Han Serif SC",
    "Source Han Serif CN",
    "STSong",
    "AR PL New Sung",
    "AR PL SungtiL GB",
    "NSimSun",
    "SimSun",
    "TW-Sung",
    "WenQuanYi Bitmap Song",
    "AR PL UMing CN",
    "AR PL UMing HK",
    "AR PL UMing TW",
    "AR PL UMing TW MBE",
    "PMingLiU",image
    "MingLiU",
    "serif";
}
.slidev-layout td {
  padding-top: 0.2em;
  padding-bottom: 0.2em;
}
table {
  margin-top: -15px;
}
</style>

---
preload: false
---

# Procedure

<span class="tracking-normal font-serif text-xl font-bold">项目测试的基本流程</span>

<div class="absolute top-0 right-0 w-60 mt-6">
  <div class="relative w-40 h-40">
    <img
      v-motion
      :initial="{ x: 800, y: -100, scale: 1.5, rotate: -50 }"
      :enter="final"
      class="absolute top-0 left-0 right-0 bottom-0"
      src="https://sli.dev/logo-square.png"
    />
    <img
      v-motion
      :initial="{ y: 500, x: -100, scale: 2 }"
      :enter="final"
      class="absolute top-0 left-0 right-0 bottom-0"
      src="https://sli.dev/logo-circle.png"
    />
    <img
      v-motion
      :initial="{ x: 600, y: 400, scale: 2, rotate: 100 }"
      :enter="final"
      class="absolute top-0 left-0 right-0 bottom-0"
      src="https://sli.dev/logo-triangle.png"
    />
  </div>
</div>
<script setup lang="ts">
const final = {
  x: 0,
  y: 0,
  rotate: 0,
  scale: 1,
  transition: {
    type: 'spring',
    damping: 10,
    stiffness: 20,
    mass: 2
  }
}
</script>

<div class="bg-slate-200 w-3/4 p-4" v-click="1">
<span class="font-mono text-base">项目测试流程分为<span class="bg-amber-300 mx-1 font-bold">项目开发阶段测试</span>和<span class="bg-amber-300 mx-1 font-bold">项目完工验收测试</span>两个阶段</span>

<span class="font-mono text-base">开发阶段测试包括：</span><br>
&nbsp;&nbsp;&nbsp;&nbsp;<span class="font-mono text-sm">1. 模块功能测试 `确保系统各功能模块能正常运行并满足需求`</span><br>
&nbsp;&nbsp;&nbsp;&nbsp;<span class="font-mono text-sm">2. 集成测试 `系统各模块组装后，能够根据业务流程需要正常完成各业务功能`</span><br>
&nbsp;&nbsp;&nbsp;&nbsp;<span class="font-mono text-sm">3. 文档检查 `对提交的项目文档和记录进行检查和验证`</span><br>

<span class="font-mono text-base">完工验收阶段的测试包括：</span><br>
&nbsp;&nbsp;&nbsp;&nbsp;<span class="font-mono text-sm">1. 安装测试 `根据项目提供的安装文档，搭建系统运行环境，检查系统安装是否成功`</span><br>
&nbsp;&nbsp;&nbsp;&nbsp;<span class="font-mono text-sm">2. 需求验证 `检查产品是否满足该项目需求说明书中规定的需求以及需求的完整性、一致性。`</span><br>
&nbsp;&nbsp;&nbsp;&nbsp;<span class="font-mono text-sm">3. 功能验证 `检查各项功能的可运行性和正确性。` <span class="bg-red-200 mx-1 font-bold">这是本次实验我们的测试方向。</span></span><br>
&nbsp;&nbsp;&nbsp;&nbsp;<span class="font-mono text-sm">4. 性能测试 `模拟多种正常、峰值以及异常负载条件来对系统的各项性能指标进行测试`</span><br>
</div>

---
preload: false
---

# Procedure

<span class="tracking-normal font-serif text-xl font-bold">项目测试的基本流程</span>

<div class="absolute top-0 right-0 w-60 mt-6">
  <div class="relative w-40 h-40">
    <img
      class="absolute top-0 left-0 right-0 bottom-0"
      src="https://sli.dev/logo-square.png"
    />
    <img
      class="absolute top-0 left-0 right-0 bottom-0"
      src="https://sli.dev/logo-circle.png"
    />
    <img
      class="absolute top-0 left-0 right-0 bottom-0"
      src="https://sli.dev/logo-triangle.png"
    />
  </div>
</div>

<div class="bg-slate-200 w-3/4 p-4">
<span class="font-mono text-sm inline-block py-2" v-click="1">1. 项目测试启动：项目立项后，在测试配置库中创建项目。<carbon:arrow-right class="inline-block pl-1"/><strong>立项</strong></span><br>
<span class="font-mono text-sm inline-block py-2" v-click="2">2. 测试计划：系统详细设计后，制定测试计划，准备测试资源。<carbon:arrow-right class="inline-block pl-1"/><strong>指定测试方案</strong></span><br>
<span class="font-mono text-sm inline-block py-2" v-click="3">3. 设计测试用例，主要是与业务相关的测试用例。<carbon:arrow-right class="inline-block pl-1"/><strong>设计测试用例</strong></span><br>
<span class="font-mono text-sm inline-block py-2" v-click="4">4. 实施功能模块测试，搭建运行或开发环境，采用功能模块测试表的方式，开发人员在功能模块测试表中更新进度状态，测试人员在该表中描述测试进度。形成测试错误列表，该表对每个错误都有相应的测试记录与之链接，在测试记录中，详细描述错误的情况。在测试记录中还要包括修正信息和验证信息。<carbon:arrow-right class="inline-block pl-1"/><strong>进行测试，反映缺陷</strong></span><br>
<span class="font-mono text-sm inline-block py-2" v-click="5">5. 错误关闭后，测试人员维护测试记录表和更新测试用例库和问题库，作为经验积累。<carbon:arrow-right class="inline-block pl-1"/><strong>完善文档</strong></span><br>
<span class="font-mono text-sm inline-block py-2" v-click="6">6. 项目在结项时，测试人员进行项目完工验收测试，填写项目测试报告。该测试报告可作为用户验收的输入工件。<carbon:arrow-right class="inline-block pl-1"/><strong>测试总结</strong></span><br>
</div>

---

# Course Targets

<span class="tracking-normal font-serif text-lg font-bold">以实际项目为抓手，运用我们在软件测试课程中所学习的方法和技能，寻找软件中存在的缺陷。</span>

📒 <span class="font-serif text-base font-bold">了解软件测试的相关知识</span> <br>
🧰 <span class="font-serif text-base font-bold">训练软件测试的方法与技能</span> <br>
💊 <span class="font-serif text-base font-bold">寻找项目存在的漏洞和缺陷</span>

<div class="flex mt-4">
  <img border="rounded" src="/sys.png" class="h-72 w-120 border-1">
  <div class="ml-12 mt-4">
    <ul class="font-mono"><span class="text-xl">功能测试</span>
      <li> 档案管理 <carbon:arrow-right class="inline-block pl-1"/> 张世豪  </li>
      <li> 培训管理 <carbon:arrow-right class="inline-block pl-1"/> 龙添辉 </li>
      <li> 奖惩管理 <carbon:arrow-right class="inline-block pl-1"/> 唐胜宇 </li>
      <li> 薪资管理 <carbon:arrow-right class="inline-block pl-1"/> 李正大 </li>
      <li> 考勤管理 <carbon:arrow-right class="inline-block pl-1"/> 唐亲贤 </li>
      <li> 请假管理 <carbon:arrow-right class="inline-block pl-1"/> 亓祺 </li>
      <li> 操作员管理 <carbon:arrow-right class="inline-block pl-1"/> 亓祺 </li>
    </ul>
  </div>
</div>

<style>
p {
  margin-bottom: 0.5em !important;
}
</style>

---
clicks: 5
---

# Personal Work

<span class="tracking-normal font-serif text-xl font-bold">个人工作的具体情况及内容</span>

<div class="flex">
  <div class="w-1/2">
  <span v-click="1" class="tracking-normal font-mono text-lg">1. 了解并选择测试项目</span><br>
  &nbsp;&nbsp;&nbsp;&nbsp;<span v-click="1" class="tracking-normal font-mono text-sm">(1) 确定测试内容</span><br>
  &nbsp;&nbsp;&nbsp;&nbsp;<span v-click="1" class="tracking-normal font-mono text-sm">(2) 选择测试策略与方法</span><br>
  &nbsp;&nbsp;&nbsp;&nbsp;<span v-click="1" class="tracking-normal font-mono text-sm">(3) 完成团队人员和任务分工</span><br>
  &nbsp;&nbsp;&nbsp;&nbsp;<span v-click="1" class="tracking-normal font-mono text-sm font-bold">成果物：《软件测试计划说明书》</span><br>

  <span v-click="2" class="tracking-normal font-mono text-lg">2. 认识软件测试行业和发展趋势</span><br>
  &nbsp;&nbsp;&nbsp;&nbsp;<span v-click="2" class="tracking-normal font-mono text-sm">(1) 学习软件测试的方法和技能</span><br>
  &nbsp;&nbsp;&nbsp;&nbsp;<span v-click="2" class="tracking-normal font-mono text-sm">(2) 认识软测行业及其发展趋势</span><br>
  &nbsp;&nbsp;&nbsp;&nbsp;<span v-click="2" class="tracking-normal font-mono text-sm">(3) 介绍自己掌握情况</span><br>
  &nbsp;&nbsp;&nbsp;&nbsp;<span v-click="2" class="tracking-normal font-mono text-sm font-bold">成果物：项目答辩1</span><br>

  </div>

  <div class="ml-8">
  <span v-click="3" class="tracking-normal font-mono text-lg">3. 编写本次测试的测试用例</span><br>
  &nbsp;&nbsp;&nbsp;&nbsp;<span v-click="3" class="tracking-normal font-mono text-sm">(1) 确定功能测试的测试用例</span><br>
  &nbsp;&nbsp;&nbsp;&nbsp;<span v-click="3" class="tracking-normal font-mono text-sm font-bold">成果物：《软件测试用例设计说明书》</span><br>

  <span v-click="4" class="tracking-normal font-mono text-lg">4. 对系统进行测试</span><br>
  &nbsp;&nbsp;&nbsp;&nbsp;<span v-click="4" class="tracking-normal font-mono text-sm">(1) 基于测试用例进行功能测试</span><br>
  &nbsp;&nbsp;&nbsp;&nbsp;<span v-click="4" class="tracking-normal font-mono text-sm">(2) 获取测试结果，掌握系统存在的缺陷</span><br>
  &nbsp;&nbsp;&nbsp;&nbsp;<span v-click="4" class="tracking-normal font-mono text-sm font-bold">成果物：《测试结果与缺陷报告书》</span><br>

  <span v-click="5" class="tracking-normal font-mono text-lg">5. 总结本次软件测试过程</span><br>
  &nbsp;&nbsp;&nbsp;&nbsp;<span v-click="5" class="tracking-normal font-mono text-sm">(1) 分析软件测试结果</span><br>
  &nbsp;&nbsp;&nbsp;&nbsp;<span v-click="5" class="tracking-normal font-mono text-sm">(2) 分析本次团队协作情况</span><br>
  &nbsp;&nbsp;&nbsp;&nbsp;<span v-click="5" class="tracking-normal font-mono text-sm font-bold">成果物：《测试总结报告》</span><br>
  </div>
</div>

---
clicks: 5
---

# Defective Code

<span class="tracking-normal font-serif text-lg font-bold">项目中的缺陷代码展示</span>

<img v-click="0" class="absolute top-20 right-12 z-50 w-120" src="/page.png">

<div v-click="1">
```java {all|11,21|12-20|all}
/**
  * 认证用户 token 登入
  * @param ServletRequest
  * @param ServletResponse
  * @return Bolean
  */
protected boolean onAccessDenied(ServletRequest request, ServletResponse response) {
  // 1. 检查请求头中是否含有token
  String token = null;
  HttpServletRequest httpServletRequest = (HttpServletRequest) request;
  // 2. 从 Cookies 中获取 token ......
  // 3. 如果客户端没有携带 token, 拦下请求
  if (token == null) {
    token = httpServletRequest.getParameter("token");
    if (ObjectUtils.isEmpty(token)) {
      log.error("未携带Token，禁止访问接口" + ((HttpServletRequest) request).getRequestURI());
      tokenError(response, "未携带Token，禁止访问接口");
      return false;
    }
  }
  // 4. 如果有，对进行进行token验证 ......
}
```
</div>

<arrow v-click="5" x1="400" y1="420" x2="230" y2="320" color="#564" width="3" arrowSize="1" />

<style>
.footnotes-sep {
  @apply mt-20 opacity-10;
}
.footnotes {
  @apply text-sm opacity-75;
}
.footnote-backref {
  display: none;
}
</style>

---
clicks: 1
---

# Defective Code

<span class="tracking-normal font-serif text-lg font-bold">登录失败问题的解决</span>

<div grid="~ cols-2 gap-4">
  <div class="bg-slate-100 rounded p-2">
    <span class="font-mono text-base">问题判断：</span> 
    <br>
    <span class="font-mono text-base">1. 抓包查看网络请求，发现前端并没有问题</span>
    <br>
    <span class="font-mono text-base">2. 查看日志发现是系统安全认证部分的问题</span>
    <br>
    <span class="font-mono text-base">3. 定位到网络请求过滤器，判断代码逻辑</span>
    <br>
    <br>
    <span class="font-mono text-base">问题定位：</span>
    <br>
    <span class="font-mono text-base">首页需验证token，但初次进入时浏览器中未保存token</span>
    <br>
    <br>
    <span class="font-mono text-base">问题解决思路：</span> <br>
    <span class="font-mono text-sm">1. 创建路由白名单</span> <br>
    <span class="font-mono text-sm">2. 当匹配到白名单中的路由，不进行验证</span>
  </div>
  <div v-click="1">
```java
protected boolean onAccessDenied(ServletRequest request, ServletResponse response) {
  // 增加判断请求路径是否在白名单中
  if (
    httpServletRequest.getRequestURI().
    equals("/")
    || httpServletRequest.getRequestURI().
    equals("/favicon.ico")
    ) {
    return true;
  }
  // 2. 如果客户端没有携带token，拦下请求
  // 3. 如果有，对进行进行token验证
}
```
  </div>
</div>

<arrow v-click="1" x1="800" y1="500" x2="650" y2="380" color="#564" width="3" arrowSize="1" />

---
layout: center
class: text-center
---

# <span class="text-7xl">End</span>


