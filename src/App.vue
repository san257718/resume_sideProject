<script setup lang="ts">
const skills = [
  "Vue 3",
  "React / Next.js",
  "TypeScript",
  "Angular",
  "Tailwind CSS",
  "Java / Spring",
  "Node.js",
  "MySQL / Oracle",
];
const specialties = [
  {
    title: "Front End",
    subtitle: "介面開發・狀態管理・效能優化",
    skills: [
      "TypeScript / JavaScript ES6+",
      "React / Next.js（App Router、SSR）",
      "Vue 3 Composition API / Nuxt 2",
      "Angular 14",
      "Zustand、Redux Toolkit、Vuex、Pinia",
      "Nx Monorepo、Custom Hooks、共用元件",
      "Tailwind CSS、SCSS、RWD、跨瀏覽器調校",
      "Ant Design、PrimeVue、Material UI、vxe-table",
      "WebSocket、Zod、React Hook Form、i18n",
    ],
  },
  {
    title: "Back End",
    subtitle: "API 設計・資料庫・部署維護",
    skills: [
      "Java、Spring Boot、Spring Data JPA",
      "Node.js、Express、RESTful API",
      "JWT 身分驗證與權限控管",
      "MySQL、Oracle、MongoDB",
      "SQL、CRUD、資料模型與欄位維護",
      "Docker 容器化與開發環境維護",
      "Vercel CI/CD、自動部署與跨網域 API 串接",
    ],
  },
];
const projects = [
  {
    number: "01",
    title: "企業管理後台",
    type: "全端開發 · 進行中",
    text: "以 React + TypeScript 建構模組化後台，整合 Material UI、Zustand 與 React Hook Form；後端使用 node、JWT 與 Mongodb，並以 Vercel 建置部署流程，後續更改為本地MySQL 與 Spring Boot + Spring Data JPA + Docker。",
    tags: ["React", "Spring Boot", "MySQL", "Docker"],
  },
  {
    number: "02",
    title: "即時匯率管理與紅包互動",
    type: "前端開發 · 商業專案",
    text: "透過 WebSocket 更新匯率資料，並實作互動式開紅包動畫；使用 Promise.all 優化錢包轉點流程，降低 API 呼叫順序造成的問題。",
    tags: ["Next.js", "WebSocket", "Zustand", "Animation"],
  },
];
const experience = [
  {
    date: "2026.04 — NOW",
    title: "皇霖實業股份有限公司",
    role: "全端工程師｜外派至 Tata Consultancy Services",
    detail:
      "維護企業專案、中文化調整與資料庫欄位修改；使用 Angular 14、Java、Oracle 與 Docker。",
  },
  {
    date: "2025.11 — 2026.06",
    title: "接案公司",
    role: "前端工程師",
    detail:
      "使用 Vue、vxe-table 與 PrimeVue 開發 SO 編輯、檢視及可搜尋的自動完成輸入功能。",
  },
  {
    date: "2024.01 — 2025.11",
    title: "無名科技有限公司",
    role: "前端工程師",
    detail:
      "以 Next.js、TypeScript、Redux、Zustand 與 Tailwind 開發前後台，參與 Nx Monorepo、表單驗證及互動功能。",
  },
  {
    date: "2022.06 — 2023.06",
    title: "通盈盛科技有限公司",
    role: "前端工程師",
    detail:
      "參與 Nuxt 2、Vue 2 專案，負責 RWD 頁面、跨瀏覽器相容與前後台功能開發。",
  },
];
</script>

<template>
  <div
    class="relative mx-auto max-w-[1440px] overflow-hidden px-[8.2%] max-[900px]:px-[5%] max-[650px]:px-[6%]"
  >
    <div
      class="absolute z-0 animate-[float_5s_ease-in-out_infinite] font-mono text-[#9dc8b1] top-[220px] left-[4%] text-[17px] max-[650px]:top-[165px] max-[650px]:left-[2%]"
    >
      ✳
    </div>
    <div
      class="absolute z-0 animate-[float_5s_ease-in-out_infinite] font-mono text-[#9dc8b1] top-[355px] right-[5%] text-[14px] [animation-delay:-2s] max-[650px]:top-[490px] max-[650px]:right-[2%]"
    >
      { }
    </div>
    <div
      class="absolute z-0 animate-[float_5s_ease-in-out_infinite] font-mono text-[#9dc8b1] top-[1040px] right-[8%] text-[22px] [animation-delay:-3s]"
    >
      ＋
    </div>
    <header
      class="relative z-10 flex h-[86px] items-center justify-between border-b border-line max-[650px]:h-[70px]"
    >
      <a
        class="inline-flex items-center gap-[9px] text-[11px] font-bold tracking-[.12em]"
        href="#home"
        ><span
          class="grid size-[30px] place-items-center rounded-lg bg-[#dceee5] font-mono text-[10px] font-medium tracking-[-.08em] text-[#426e5b]"
          >LW</span
        >
        LI WEN-YI <i>·</i> DEV</a
      >
      <nav
        class="flex items-center gap-[33px] text-[11px] text-[#627176] max-[650px]:gap-[14px] max-[650px]:text-[9px] [&>a]:transition-colors [&>a:hover]:text-green [&>a:first-child]:max-[650px]:hidden"
        aria-label="主要導覽"
      >
        <a href="#about">關於</a><a href="#experience">經歷</a
        ><a href="#work">專案</a
        ><a
          href="#contact"
          class="rounded-md border border-[#d7e3dd] px-[15px] py-[10px] text-ink max-[650px]:px-[10px] max-[650px]:py-2"
          >聯絡我 <span>↗</span></a
        >
      </nav>
    </header>

    <main>
      <section
        id="home"
        class="relative grid min-h-[620px] grid-cols-[1.05fr_.95fr] items-center px-[4%] pt-[35px] pb-[82px] max-[900px]:min-h-[580px] max-[900px]:px-[1%] max-[650px]:min-h-0 max-[650px]:grid-cols-1 max-[650px]:px-0 max-[650px]:pt-[52px] max-[650px]:pb-[75px]"
      >
        <div class="relative z-[1] animate-[rise_.8s_both]">
          <div
            class="flex items-center gap-[10px] font-mono text-[9px] font-medium tracking-[.14em] text-[#6e8a7b]"
          >
            <span
              class="size-[7px] rounded-full bg-[#6dba8e] shadow-[0_0_0_4px_#e1f0e7]"
            ></span>
            FRONTEND · FULL-STACK DEVELOPER
          </div>
          <h1
            class="my-[29px] mb-[17px] text-[62px] font-bold leading-[1.27] tracking-[-.06em] max-[900px]:text-[53px] max-[650px]:my-6 max-[650px]:text-[52px]"
          >
            你好，我是<br /><span class="text-[#3d745d]">李文儀</span
            ><span
              class="ml-[15px] mt-[15px] inline-block origin-center align-top font-mono text-[27px] text-[#82b89e] animate-[wave_3s_ease-in-out_infinite]"
              >⌘</span
            >
          </h1>
          <p class="text-base font-medium leading-[1.95] max-[650px]:text-sm">
            專注打造<span>穩定、直覺</span>的 Web 使用體驗。<br />具備前端開發與全端整合經驗。
          </p>
          <p class="mt-[13px] font-mono text-[12px] text-muted">
            3–4 年開發經驗 · 持續探索更好的解法。
          </p>
          <div class="mt-7 flex items-center gap-[25px]">
            <a
              class="inline-flex items-center gap-[18px] rounded-[5px] bg-[#47775f] px-[18px] py-[14px] text-[12px] font-semibold text-white transition duration-200 hover:-translate-y-[3px] hover:shadow-[0_9px_20px_#426f5b29]"
              href="#work"
              >探索專案 <span>↓</span></a
            ><a
              class="text-[12px] font-semibold transition-colors hover:text-green"
              href="#contact"
              >與我聯絡 <span>↗</span></a
            >
          </div>
        </div>
        <div
          class="relative grid h-[420px] place-items-center animate-[rise_.8s_both] [animation-delay:.18s] max-[900px]:scale-[.88] max-[650px]:mt-[26px] max-[650px]:h-[340px] max-[650px]:scale-90"
        >
          <div
            class="orbit-one absolute h-[310px] w-[390px] rounded-full border border-[#cbded4] animate-[orbit_18s_linear_infinite] max-[650px]:h-[260px] max-[650px]:w-[320px]"
          ></div>
          <div
            class="orbit-two absolute h-[385px] w-[320px] rotate-[32deg] rounded-full border border-[#e0e9e4] animate-[orbit-reverse_22s_linear_infinite] max-[650px]:h-[325px] max-[650px]:w-[270px]"
          ></div>
          <div
            class="relative z-[1] w-[340px] rotate-[-2deg] overflow-hidden rounded-lg border border-[#3c4e53] bg-[#25343c] shadow-[0_22px_60px_#263c3826] animate-[card-float_6s_ease-in-out_infinite] max-[650px]:w-[min(340px,90vw)]"
          >
            <div
              class="flex h-[39px] items-center border-b border-[#405057] bg-[#2d3d44] px-[13px] font-mono text-[9px] text-[#a0b1ae]"
            >
              <div class="mr-[22px] flex gap-[5px]"><i></i><i></i><i></i></div>
              <span>about-me.ts</span><b>•••</b>
            </div>
            <div
              class="px-5 pt-[17px] pb-[19px] font-mono text-[10px] leading-[1.85] text-[#b7c4c0]"
            >
              <span class="mb-[9px] block text-[9px] text-[#799189]"
                >// 一點好奇心，很多實作</span
              >
              <p class="m-0"><b>const</b> developer = {</p>
              <p class="pl-[17px]">
                <span>name</span>:
                <em class="not-italic text-green">'李文儀'</em>,
              </p>
              <p class="pl-[17px]">
                <span>focus</span>:
                <em class="not-italic text-green">'Web 開發'</em>,
              </p>
              <p class="pl-[17px]"><span>stack</span>: [</p>
              <p class="indent more">
                <em class="not-italic text-green">'Vue'</em>,
                <em class="not-italic text-green">'React'</em>,
              </p>
              <p class="indent more">
                <em class="not-italic text-green">'TypeScript'</em>,
                <em class="not-italic text-green">'Java'</em>
              </p>
              <p class="pl-[17px]">],</p>
              <p class="pl-[17px]"><span>status</span>: <i>true</i></p>
              <p class="m-0">};</p>
              <div
                class="mt-[15px] border-t border-[#405057] pt-3 text-[8px] text-[#96aaa3]"
              >
                <span>➜</span> building something useful<span
                  class="text-[#b0dfbf] animate-[blink_1s_steps(2)_infinite]"
                  >_</span
                >
              </div>
            </div>
            <div
              class="flex h-[29px] items-center justify-between border-t border-[#405057] px-[13px] font-mono text-[7px] tracking-[.08em] text-[#7c9990]"
            >
              <span>● SYSTEM ONLINE</span><span>v. 2026</span>
            </div>
          </div>
          <div
            class="absolute z-[2] flex items-center gap-[10px] rounded-md border border-[#e0e9e4] bg-white px-[14px] py-[11px] text-[8px] leading-[1.5] text-[#6e7d7c] shadow-[0_8px_24px_#26433d12] top-[51px] right-px rotate-[4deg] max-[650px]:top-[30px] max-[650px]:right-[-3px]"
          >
            <b>5+</b><span>frameworks<br />in practice</span>
          </div>
          <div
            class="absolute z-[2] flex items-center gap-[10px] rounded-md border border-[#e0e9e4] bg-white px-[14px] py-[11px] text-[8px] leading-[1.5] text-[#6e7d7c] shadow-[0_8px_24px_#26433d12] bottom-10 left-0 -rotate-[4deg] max-[650px]:bottom-[25px] max-[650px]:left-[-3px]"
          >
            <span
              class="grid size-[27px] place-items-center rounded-[5px] bg-[#e1f0e7] text-[15px] text-[#538369]"
              >✦</span
            ><span>curious mind,<br /><b>careful code.</b></span>
          </div>
        </div>
        <a
          class="absolute bottom-[22px] left-1/2 flex -translate-x-1/2 items-center gap-[10px] font-mono text-[8px] tracking-[.13em] text-[#8b9995] max-[650px]:bottom-[15px]"
          href="#about"
          ><span></span> SCROLL TO EXPLORE</a
        >
      </section>

      <section
        id="about"
        class="border-t border-line px-[4%] py-[83px] max-[900px]:px-[2%] max-[650px]:py-[60px]"
      >
        <div
          class="flex items-center gap-3 font-mono text-[9px] font-medium tracking-[.14em] text-[#6e8a7b]"
        >
          <span>01</span> ABOUT ME
        </div>
        <div
          class="mt-[39px] grid grid-cols-[1.1fr_.9fr] gap-[75px] max-[900px]:gap-[35px] max-[650px]:mt-[26px] max-[650px]:grid-cols-1 max-[650px]:gap-[18px]"
        >
          <div>
            <h2
              class="m-0 text-[30px] font-semibold leading-[1.6] tracking-[-.045em] max-[650px]:text-2xl"
            >
              把複雜問題拆開，<br /><em class="not-italic text-green"
                >一步一步做好。</em
              >
            </h2>
            <div
              class="mt-[19px] font-mono text-[17px] tracking-[.35em] text-[#78a98e]"
            >
              — ✳ —
            </div>
          </div>
          <div
            class="text-[11px] leading-[2.1] text-[#69787a] max-[650px]:text-[10px]"
          >
            <p class="m-0 text-[14px]">
              我是李文儀，累積 3–4 年 Web 軟體開發經驗，主要使用
              Vue、React、Next.js 與 Angular 建置產品介面，也參與 API
              串接、狀態管理及資料庫維護。
            </p>
            <p class="mt-3 mb-0 text-[14px]">
              我重視可維護的元件與穩定的使用體驗，曾參與即時資料、複雜表格、表單驗證與前後端分離專案，並持續拓展
              Java、Spring Boot 與 Node.js 的實作能力。
            </p>
            <div class="mt-[18px] flex flex-wrap gap-2">
              <span
                class="rounded bg-[#eaf1ed] px-[10px] py-[7px] text-[12px] text-[#63746f]"
                >📍 台北・中山</span
              ><span
                class="rounded bg-[#eaf1ed] px-[10px] py-[7px] text-[12px] text-[#63746f]"
                >💻 前端 / 全端</span
              ><span
                class="rounded bg-[#eaf1ed] px-[10px] py-[7px] text-[12px] text-[#63746f]"
                >🧩 持續學習中</span
              >
            </div>
          </div>
        </div>
      </section>

      <section
        class="border-t border-line bg-[#eef4f0] px-[4%] pt-[57px] pb-[59px] max-[900px]:px-[2%] max-[650px]:py-[60px]"
      >
        <div
          class="flex items-center gap-3 font-mono text-[9px] font-medium tracking-[.14em] text-[#6e8a7b]"
        >
          <span>02</span> TECH TOOLKIT
        </div>
        <div
          class="mt-[25px] grid grid-cols-[.65fr_1.35fr] items-center max-[650px]:grid-cols-1 max-[650px]:gap-[18px]"
        >
          <h2
            class="m-0 text-[22px] font-semibold leading-[1.6] tracking-[-.045em] max-[650px]:text-xl"
          >
            常用技術
          </h2>
          <div class="flex flex-wrap gap-2 max-[650px]:gap-[7px]">
            <span
              v-for="(skill, i) in skills"
              :key="skill"
              :class="[
                'rounded border border-[#d6e3dc] bg-[#f9fbf9] px-[11px] py-[9px] font-mono text-[9px] text-[#52645d] transition hover:-translate-y-[3px] hover:bg-white',
                i === 1 || i === 4 ? 'translate-y-1' : '',
              ]"
              >{{ skill }} <b>✳</b></span
            >
          </div>
        </div>
      </section>

      <section class="border-t border-line px-[4%] py-[83px] max-[900px]:px-[2%] max-[650px]:py-[60px]">
        <div class="flex items-center gap-3 font-mono text-[9px] font-medium tracking-[.14em] text-[#6e8a7b]">
          <span>03</span> TECHNICAL SPECIALTIES
        </div>
        <div class="mt-6 grid grid-cols-2 gap-5 max-[650px]:grid-cols-1">
          <article v-for="specialty in specialties" :key="specialty.title" class="rounded-md border border-[#e0e8e3] bg-white p-6 max-[650px]:p-5">
            <div class="flex items-start justify-between gap-3">
              <h2 class="m-0 text-[25px] font-semibold tracking-[-.04em] text-[#3d745d]">{{ specialty.title }}</h2>
              <span class="mt-1 rounded bg-[#eaf1ed] px-2 py-1 font-mono text-[8px] tracking-[.06em] text-[#63746f]">SPECIALTY</span>
            </div>
            <p class="mt-1 mb-0 text-[10px] text-[#82908f]">{{ specialty.subtitle }}</p>
            <ul class="mt-5 grid gap-3 border-t border-[#e8eeea] pt-5">
              <li v-for="item in specialty.skills" :key="item" class="flex items-start gap-2 text-[14px] leading-[1.7] text-[#52645d]">
                <span class="mt-[5px] size-[6px] shrink-0 rounded-full bg-[#6eaa89]"></span>{{ item }}
              </li>
            </ul>
          </article>
        </div>
      </section>

      <section
        id="experience"
        class="grid grid-cols-[.75fr_1.25fr] gap-11 border-t border-line px-[4%] py-[83px] max-[900px]:px-[2%] max-[650px]:grid-cols-1 max-[650px]:gap-5 max-[650px]:py-[60px]"
      >
        <div>
          <div
            class="flex items-center gap-3 font-mono text-[9px] font-medium tracking-[.14em] text-[#6e8a7b]"
          >
            <span>04</span> EXPERIENCE
          </div>
          <h2
            class="mt-6 mb-0 text-[23px] font-semibold leading-[1.6] tracking-[-.045em] max-[650px]:text-[21px]"
          >
            一路累積的實戰經驗
          </h2>
          <p
            class="mt-[10px] max-w-[270px] text-[14px] leading-[1.9] text-[#82908f]"
          >
            從 Vue/Nuxt 到 React/Next，再延伸至企業系統與全端整合。
          </p>
        </div>
        <div class="mt-[3px] ml-[6px] border-l border-[#ccdbd2]">
          <article
            v-for="job in experience"
            :key="job.title"
            class="relative grid grid-cols-[110px_1fr_18px] gap-3 pb-[23px] pl-5 last:pb-0 max-[900px]:grid-cols-[96px_1fr_15px] max-[650px]:grid-cols-[86px_1fr_13px] max-[650px]:gap-2 max-[650px]:pl-4"
          >
            <span
              class="pt-[3px] font-mono text-[8px] tracking-[.04em] text-[#718f7f]"
              >{{ job.date }}</span
            >
            <div>
              <h3 class="mb-1 text-[11px] font-semibold">{{ job.title }}</h3>
              <b>{{ job.role }}</b>
              <p
                class="mt-[6px] mb-0 text-[12px] leading-[1.75] text-[#7e8a89] max-[650px]:text-[8px]"
              >
                {{ job.detail }}
              </p>
            </div>
            <span class="text-xs text-[#73a487]">✳</span>
          </article>
        </div>
      </section>

      <section
        id="work"
        class="border-t border-line bg-[#f1f5f2] px-[4%] pt-[79px] pb-[87px] max-[900px]:px-[2%] max-[650px]:py-[60px]"
      >
        <div
          class="mt-[23px] mb-[29px] flex items-end justify-between max-[650px]:mb-[23px] max-[650px]:block"
        >
          <div>
            <div
              class="flex items-center gap-3 font-mono text-[9px] font-medium tracking-[.14em] text-[#6e8a7b]"
            >
              <span>05</span> SELECTED PROJECTS
            </div>
            <h2
              class="mt-[10px] mb-0 text-[26px] font-semibold leading-[1.6] tracking-[-.045em] max-[650px]:text-[23px]"
            >
              專案與成果<span class="text-[#679c7d]"> ✳</span>
            </h2>
          </div>
          <p
            class="m-0 mb-[3px] text-[12px] leading-[1.9] text-[#82908f] max-[650px]:mt-2"
          >
            將產品需求轉成可維護、<br />可持續迭代的功能。
          </p>
        </div>
        <div
          class="grid grid-cols-2 gap-[19px] max-[650px]:grid-cols-1 max-[650px]:gap-[14px]"
        >
          <article
            v-for="project in projects"
            :key="project.number"
            class="overflow-hidden rounded-md border border-[#e0e8e3] bg-white transition duration-200 hover:-translate-y-[5px] hover:shadow-[0_16px_32px_#365b4915]"
          >
            <div
              class="relative grid h-[240px] place-items-center overflow-hidden max-[650px]:h-[220px]"
              :class="project.number === '01' ? 'bg-[#e6efe9]' : 'bg-[#26373e]'"
            >
              <span
                class="absolute top-[14px] left-4 font-mono text-[8px] tracking-[.1em] text-[#778d81]"
                >PROJECT_{{ project.number }}</span
              ><template v-if="project.number === '01'"
                ><div class="dashboard">
                  <div class="dash-side">
                    <span>◈</span><i></i><i></i><i></i>
                  </div>
                  <div class="dash-main">
                    <span class="dash-title">Overview <b>•••</b></span>
                    <div class="dash-metrics">
                      <span
                        ><i>總使用者</i><b>2,486</b><small>↗ 12.8%</small></span
                      ><span
                        ><i>本月營收</i><b>$48,290</b
                        ><small>↗ 8.2%</small></span
                      >
                    </div>
                    <div class="chart">
                      <span></span><span></span><span></span><span></span
                      ><span></span><span></span><span></span><span></span
                      ><span></span><span></span><span></span><span></span>
                    </div>
                  </div>
                </div>
                <span
                  class="absolute right-4 bottom-[14px] font-mono text-[8px] text-[#769181]"
                  >react + spring boot</span
                ></template
              ><template v-else
                ><div class="code-window">
                  <div class="code-title">
                    <i></i><i></i><i></i><span>realtime.ts</span>
                  </div>
                  <div class="code-lines">
                    <span
                      ><b>01</b>
                      <em class="not-italic text-green">socket</em
                      >.on(<strong>'rate:update'</strong>,</span
                    ><span
                      ><b>02</b> &nbsp; (data) =&gt;
                      <em class="not-italic text-green">setRate</em>(data)</span
                    ><span><b>03</b> );</span><span><b>04</b></span
                    ><span
                      ><b>05</b>
                      <em class="not-italic text-green">Promise</em
                      >.all(tasks)</span
                    >
                  </div>
                </div>
                <span class="visual-note"
                  >websocket · smooth flow</span
                ></template
              >
            </div>
            <div
              class="grid grid-cols-[1fr_20px] items-start p-[18px] px-[19px] pb-[19px]"
            >
              <div>
                <span
                  class="font-mono text-[10px] tracking-[.06em] text-[#789182]"
                  >{{ project.type }}</span
                >
                <h3 class="mt-[6px] mb-0 text-md font-semibold">
                  {{ project.title }}
                </h3>
              </div>
              <span
                class="text-base text-[#57836c] transition-transform group-hover:translate-x-0.5 group-hover:-translate-y-0.5"
                >↗</span
              >
              <p
                class="col-span-2 m-0 my-[11px] text-[11px] leading-[1.9] text-[#75817e]"
              >
                {{ project.text }}
              </p>
              <div class="col-span-2 flex flex-wrap gap-[6px]">
                <span v-for="tag in project.tags" :key="tag">{{ tag }}</span>
              </div>
            </div>
          </article>
        </div>
      </section>

      <section
        class="border-t border-line px-[4%] pt-[63px] pb-[63px] max-[900px]:px-[2%] max-[650px]:py-[52px]"
      >
        <div
          class="flex items-center gap-3 font-mono text-[9px] font-medium tracking-[.14em] text-[#6e8a7b]"
        >
          <span>06</span> EDUCATION
        </div>
        <div
          class="mt-[22px] flex max-w-[550px] items-center gap-[14px] rounded-[5px] border border-[#e2e9e5] bg-white px-[18px] py-4"
        >
          <span
            class="grid size-[35px] place-items-center rounded-[5px] bg-[#e9f2ec] text-[17px] text-[#5a866c]"
            >◫</span
          >
          <div>
            <h3 class="mb-1 text-[14px] font-semibold">朝陽科技大學</h3>
            <p class="m-0 text-[11px] text-[#788683]">企業管理系｜四技肄業</p>
          </div>
          <span class="ml-auto font-mono text-[8px] text-[#80918a]"
            >2009 — 2014</span
          >
        </div>
      </section>

      <section
        id="contact"
        class="border-t border-line px-[4%] pt-[74px] pb-[76px] max-[900px]:px-[2%] max-[650px]:py-[60px]"
      >
        <div
          class="relative overflow-hidden rounded-[5px] border border-[#dce9e0] bg-[#eaf2ed] px-5 pt-12 pb-[41px] text-center max-[650px]:px-3 max-[650px]:pt-11 max-[650px]:pb-9"
        >
          <span
            class="absolute left-[12%] top-[26%] text-[25px] text-[#78a88a] max-[650px]:left-[5%] max-[650px]:top-[13%]"
            >✳</span
          ><span
            class="absolute right-[13%] bottom-[20%] text-2xl text-[#78a88a] max-[650px]:right-[5%] max-[650px]:bottom-[12%]"
            >＋</span
          >
          <div
            class="flex items-center gap-3 font-mono text-[9px] font-medium tracking-[.14em] text-[#6e8a7b]"
          >
            <span>07</span> LET'S CONNECT
          </div>
          <h2
            class="relative z-[1] mt-[15px] mb-0 text-[28px] font-semibold leading-[1.6] tracking-[-.045em] max-[650px]:text-[23px]"
          >
            一起把好點子<span class="contact-underline relative text-[#47775f]"
              >做出來。</span
            >
          </h2>
          <p
            class="relative mt-[11px] mb-5 text-[12px] leading-[2] text-[#708079] max-[650px]:text-[9px]"
          >
            期待加入重視合作與持續改善的團隊，<br />用穩定的實作，讓產品體驗持續變好。
          </p>
          <span
            class="inline-flex items-center gap-[18px] rounded-[5px] bg-[#47775f] px-[18px] py-[14px] text-[12px] font-semibold text-white transition duration-200 hover:-translate-y-[3px] hover:shadow-[0_9px_20px_#426f5b29]"
            >nokelove1111@gmail.com </span>
        </div>
      </section>
    </main>
    <footer
      class="flex h-[72px] items-center justify-between border-t border-line font-mono text-[8px] text-[#87928f] max-[650px]:h-auto max-[650px]:min-h-[69px] max-[650px]:flex-wrap max-[650px]:gap-[10px] max-[650px]:py-4"
    >
      <a
        class="inline-flex items-center gap-[9px] text-[11px] font-bold tracking-[.12em]"
        href="#home"
        ><span
          class="grid size-[30px] place-items-center rounded-lg bg-[#dceee5] font-mono text-[10px] font-medium tracking-[-.08em] text-[#426e5b]"
          >LW</span
        >
        LI WEN-YI <i>·</i> DEV</a
      ><span>Built with curiosity & care. <b>⌘</b></span
      ><span>© 2026 李文儀</span>
    </footer>
  </div>
</template>
