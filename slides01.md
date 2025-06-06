---
theme: seriph
title: 前端架構討論簡報
background: "https://images.unsplash.com/photo-1530819568329-97653eafbbfa?ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&ixlib=rb-1.2.1&auto=format&fit=crop&w=2092&q=80"
class: text-center
drawings:
  persist: false
transition: slide-left
mdc: true
---

# 前端的架構討論

沒有絕對好的架構，只有適合當下團隊的架構

<div class="abs-br m-6 text-xl">
  <a href="https://gitlab.aservice.com.tw/hepiuscare/frontend/apps/hepius-record" target="_blank" class="slidev-icon-btn">
    <carbon:logo-github />
  </a>
</div>

---

layout: image-left
image: https://source.unsplash.com/collection/94734566/1920x1080

---

# Vita 遇到了什麼架構上的問題？

<v-clicks every="1" class="full-height">

- 路由定義組件不易辨識：從各個組件當中，難以分辨其哪些是**頁面**哪些是**組件**，接手的學習成本高
- 常見核心功能沒有合適位置定義：路由常用功能 **resolve(動態請求資料)**、**guard(路由守衛)**、**store(全域狀態管理資料)** 及 **interceptors(攔截器)** 沒有合適的地方擺放
- 組件分類紊亂：沒辦法將**網頁佈局(layout)組件**清楚辨識，讓開發者專注在開發單一組件的功能
- api.reference.json 開發困境：端點跟型別分開定義，導致難以快速識別 api 功能，且後續不易擴展

</v-clicks>

<style>
.full-height{
  margin-top: 2rem;
  display: flex;
  gap: 1.5rem;
  flex-direction: column;
  font-size: 1.2rem;
}
.full-height strong {
  color: #D79B00;
}
</style>

---

# 過去版本

<v-switch>
  <template #1>
    <img src="./public/t0.png" />
  </template>
  <template class="flex" #2>
    <div class="pic">
      <img src="./public/t1.png" />
    </div>
    <div class="text">
      <ul>123</ul>
    </div>
  </template>
</v-switch>

<style>
.slidev-layout h1 + p {
  opacity: 1;
}
.slidev-vclick-hidden{
  display: none;
}
.content{
  display: flex;
}
</style>

---

# 123
