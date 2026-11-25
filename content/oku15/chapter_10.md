---
title: "OKU 15 Ch.10: New Technology — Robotics, Navigation, AR, and VR（OKU 14 CH11 拆分）"
date: 2026-11-25
draft: false
tags: ["OKU15", "General Topics", "Robotics", "Augmented Reality", "版本差異"]
categories: ["OKU 15 更新"]
weight: 10
summary: "由 OKU 14 CH11 拆出的機器人／導航／AR／VR 章（10 頁）。新增 levels of autonomy（Level 0–5）分類、open vs closed platform、美國 robotic TKA 系統總表、AR 硬體差異（marker vs markerless、holographic vs pass-through）與 AR 的 TKA／THA／rTSA／spine／trauma 數據。"
---

> **對照：**OKU 14 [CH11 New Technology（Robotics, AI, ML）]({{< relref "/chapter_11.md" >}}) 的機器人與 AR 部分 → OKU 15 **Ch.10**；AI／ML 部分另成 [Ch.11]({{< relref "/oku15/chapter_11.md" >}})｜作者群全新｜PDF 10 頁
>
> **閱讀方式：**🆕 新增；🔄 改變；✅ 一致；❌ OKU 15 不再涵蓋。

## 0. 考點變更總表

| 主題 | OKU 14 CH11 | OKU 15 Ch.10 | 類型 |
|---|---|---|---|
| 機器人分類架構 | 依運作原理分五類：active（ROBODOC）、semiactive haptic、定位 cutting guide、限制電動工具運動、accelerometer／freehand navigated | 改用 **FDA 的 levels of autonomy（Level 0–5）**，再細分 active guidance 與 passive support | 🔄 |
| 用語 | — | FDA 自 2015 年起改稱 **robotically assisted surgical devices**，強調仍由醫師控制 | 🆕 |
| Open vs closed platform | 未談 | 美國幾乎都是 **closed**；**唯一 open 平台是 THINK Surgical（TSolution-One、TMINI）** | 🆕 |
| 美國 robotic TKA 系統 | 個別介紹 | **8 套系統總表**（廠商、open/closed、active/semiactive、FDA 年份、切骨方式、影像需求） | 🆕 |
| 骨科機器人數量 | — | **骨科是 FDA 核准手術機器人最多的專科**，幾乎都走 **510(k)** 途徑 | 🆕 |
| 臨床效益數據 | Mako UKA 系統性回顧；Mako TKA 成本 $11,615 vs $8,674；iASSIST、OrthAlign | 換成：**MUA 減少 4 倍**、KSS 17 vs 15.5（3 個月）；**機器人價格 $40 萬–150 萬美元** | 🔄 |
| PSI、kinematic registration、registration 原理、國際標準 | CH11 有詳細說明 | **不再涵蓋** | ❌ |
| AR 系統 | 舉 HipInsight、ARVIS、NextAR 為例，**當時尚無臨床數據** | 已有數據：**AR-THA 的 RCT**、AR-TKA 準確度、rTSA 屍體研究、spine pedicle screw、IM nail distal locking | 🔄 |
| AR 硬體差異 | HoloLens 簡介 | **Image-based vs imageless**、**marker vs markerless**、**holographic vs pass-through**、操控方式 | 🆕 |
| AR／VR 用於復健、VR 訓練 | 簡單帶過 | 獨立段落：cybersickness、跌倒風險、觸覺回饋不足造成的 ceiling effect | 🆕 |

---

## 1. 機器人概論

### 1.1 歷史與現況
- 手術機器人始於 **1985 年**的神經外科切片導引。
- 骨科第一台是 **ROBODOC（1992 年）**，用於 THA 股骨端的 milling。後來因技術複雜、手術時間長、併發症多而**停產**，但它是現有系統的前身。
- 🆕 **骨科是 FDA 核准手術機器人數量最多的專科**，而且幾乎都經 **510(k)** 途徑核准。

### 1.2 優點與缺點 🔄
- **優點：**提高精準度與準確度，減少技術上的離群值，對高 volume 和低 volume 醫師都有幫助。過了學習曲線後，可以減輕人體工學負擔（例如不用固定切骨導板）和心理壓力，因為切骨前就能用數字確認 gap balance。
- **臨床數據：**
  - 一項 188 例 TKA 研究中，機器人組的 **MUA 發生率低 4 倍**。
  - 另一研究 3 個月時 **KSS 17 vs 15.5**（機器人 vs 傳統）。
- **缺點：**
  - **直接成本 40 萬–150 萬美元**。
  - 間接成本：病人往返影像中心、術前規劃、工程師建模、輻射暴露、軟體與維護費、耗材、人員訓練、庫存、折舊。
  - 部分保險不給付 robotic TKA 或術前 CT，在 bundled payment 下特別有壓力。

### 1.3 Image-based vs imageless ✅
- **Image-based**：需要術前 X 光、CT 或 MRI 來規劃切骨、尺寸、腿長、offset、gap。術中再用 tracker 註冊、比對 3D 模型。缺點是費用、不便，以及 CT 的輻射。
- **Imageless**：完全靠術中註冊建立模型。比較便宜方便、沒有額外輻射，但**準確度取決於醫師取點**，也無法在術前驗證模型。

### 1.4 Open vs closed platform 🆕
- **Closed**：機器人只能搭配同一家廠商的植入物（垂直整合）。**美國目前幾乎都是 closed**。
- **Open**：不限植入物廠牌。**目前唯一的 open 平台廠商是 THINK Surgical（TSolution-One、TMINI）**。
- Open 平台的缺點是缺乏個別植入物的精細模型，例如 gap 評估、雙曲率股骨元件、medial pivot。
- 產業有維持 closed 的誘因，因此要留意新舊世代的相容性和價格歧視。

### 1.5 Levels of autonomy 🆕（高頻考點）

| Level | 名稱 | 定義 |
|---|---|---|
| 0 | No autonomy | 等同傳統手術 |
| **1** | **Robot assistance** | 醫師持續控制；系統提供 **passive support**（tremor filtration、teleoperation、tool tracking）或 **active guidance**（**haptic feedback、motion boundary**） |
| 2 | Task autonomy | 醫師設定參數，系統接手執行該步驟 |
| **3** | **Conditional autonomy** | 系統產生數個方案供醫師選擇，再自行執行 |
| 4 | High-level autonomy | 系統自行選出最佳的病人專屬方案並執行 |
| 5 | Full autonomy | 系統對整個手術自行決策 |

- **幾乎所有骨科機器人都屬於 Level 1。**
- **美國市場只有一台 active robot（Level 3）**，就是 TSolution-One，臨床數據還很少。
- 本章的 key points 也提到：**除兩套系統外，其餘都是 semiactive**。

### 1.6 美國 robotic TKA 系統一覽 🆕

| 系統 | 廠商 | 平台 | 類型 | FDA | 切骨方式 | 影像 |
|---|---|---|---|---|---|---|
| TSolution-One | THINK Surgical | Open | **Active** | 2019 | Milling | CT |
| TMINI | THINK Surgical | Open | Semiactive | 2024 | Pin driver | CT |
| ROSA | Zimmer Biomet | Closed | Semiactive | 2019 | Cutting guide | X 光或 imageless |
| MAKO | Stryker | Closed | Semiactive | 2015 | Saw | CT |
| Navio | Smith & Nephew | Closed | Semiactive | 2017 | Burr | Imageless |
| CORI | Smith & Nephew | Closed | Semiactive | 2022 | Burr | Imageless |
| VELYS | DePuy Synthes | Closed | Semiactive | 2021 | Saw | Imageless |
| OMNIbotics | Corin | Closed | Semiactive | 2017 | Cutting guide 或 burr | Imageless |

> 原表的欄位排版有錯位，影像需求一欄請以原書 Table 1 為準。考試較常考的是：**MAKO 用 CT 加 saw，CORI／Navio 用 burr 且 imageless，THINK Surgical 是唯一的 open 平台，也是唯一的 active 系統**。

---

## 2. Augmented reality（AR）

### 2.1 定義 🔄
- **AR**：把電腦產生的影像投射到使用者的視野中，通常使用 **HMD**（頭戴式顯示器），也可以用手持螢幕或投影。
- **Mixed reality**：實體與虛擬物件之間可以互動，例如 HMD 顯示虛擬規劃，同時即時追蹤病人身上的 array。實務上常與 AR 混用。
- **VR**：完全沉浸，看不到真實世界，主要用在訓練。

### 2.2 硬體差異 🆕（觀念題）

| 比較 | 選項 A | 選項 B |
|---|---|---|
| 導引來源 | **Image-based**：疊合術前或術中影像，可減少術中透視，但術前影像仍有輻射 | **Imageless**：需要術中註冊。**目前骨科 AR 大多是 imageless**，因為 image-based 需要的運算與術前準備較多 |
| 追蹤方式 | **Marker-based**：以球形 array 等標記追蹤；**array 一旦被撞歪、移位或被血跡遮住，就會失準** | **Markerless**：直接辨識解剖或手部；手套沾血也可能失去追蹤。**Electromagnetic tracking** 不需要視線，適合 IM nail interlocking |
| 顯示方式 | **Holographic**：投射在透明鏡片上；**裝置故障時仍看得到術野**，但鏡片會影響視線，且需要很大運算量、頭戴溫度高 | **Pass-through**：透過 RGB-D 相機重現真實世界，色彩與整合較好；**裝置故障時會完全遮住視線** |
| 操控方式 | 手勢、眼動追蹤、語音 | 消費型產品多用遙控器 |

### 2.3 臨床應用與數據 🔄

| 術式 | 重點 |
|---|---|
| **TKA** | 多為 marker-based 加 imageless，array 以 half pin 固定在股骨和脛骨。成本與占地介於 CA-TKA 和 RA-TKA 之間，可以在術中確認骨性標記，但**骨頭仍由醫師自己切**。**平均多花約 5 分鐘**。76 例研究中，**96% 的 varus 誤差在 1° 以內**。目前缺乏與 CA 或 RA 的直接比較 |
| **THA** | **2024 年 RCT（72 例）：杯子落在 Lewinnek safe zone 的比例 94% vs 64%**；但 6 個月時**臨床分數與併發症沒有差異** |
| **Reverse TSA** | 與 TKA、THA 不同，**早期 rTSA 平台是 image-based**，用術前 CT 建立 scapula 全像圖來導引 guidewire；屍體研究顯示與規劃的偏差很小 |
| **Spine** | Image-based，術中選擇 pedicle screw 尺寸。校準時間短（約 4 分鐘），MIS 置釘準確且安全 |
| **Trauma** | Image-based 可以減少 C-arm 使用。**IM nail distal locking 只用兩張 X 光，100 秒內成功率 93%** |

### 2.4 在手術室導入 AR 的實務問題 🆕
- HMD 通常只在註冊和規劃階段戴，**無法高壓滅菌**，比照可重複使用的護目鏡處理。
- 需要第三人協助取下，因為重量會加重 **cybersickness**。
- **面罩會擋住光學追蹤，所以戴 AR 時常常不能用無菌手術頭盔**，在把頭盔列為常規的醫院會遇到行政上的阻力。
- 裝置當機時，必須能立刻改回傳統方法。

### 2.5 AR／VR 用於復健 🆕
- **AR-PT：**可以示範動作、依能力調整進度，並記錄時間、次數、困難項目等配合度數據。**限制是無法讀取病人的非語言線索**（疼痛、不適），戴 HMD 也不舒服，且有跌倒風險。
- **VR-PT：**更沉浸，可以第一人稱看到肢體，例如用於 **phantom limb pain**。但看不到真實環境，**受傷風險比 AR 更高**。

---

## 3. Virtual reality 用於訓練 🆕
- **優點：**成本低、病人沒有風險，並提供完成時間、錯誤率等客觀指標。住院醫師認為 VR 最適合 intern 和 junior 學習解剖、暴露和手術步驟。
- **限制：**
  - 多數使用一般商用硬體，**缺乏觸覺回饋**，所以會出現 **ceiling effect**。
  - 難以模擬骨骼畸形、血管變異等少見解剖。
  - 未來可能結合 AI 增加變化，但運算能力和電池續航仍是瓶頸。
- 住院醫師多半希望 VR 是**選修的輔助工具**，而不是必修課程或能力評估。

---

## 4. OKU 14 CH11 中 OKU 15 不再涵蓋的內容 ❌
- PSI（patient-specific instrumentation）與 kinematic registration
- 3D 定位、追蹤與 registration 的原理
- 依運作原理的五類機器人分類，以及 iASSIST、OrthAlign 等 accelerometer 系統的數據
- Mako UKA 系統性回顧、Mako TKA 成本比較（$11,615 vs $8,674）
- 臨床前測試與國際標準

這些內容可以當背景知識，但不是 OKU 15 的考點。

---

## 5. Anki 候選題

1. FDA 自 2015 年起建議用什麼名稱取代 surgical robot？→ Robotically assisted surgical devices。
2. 幾乎所有骨科機器人屬於哪一個 autonomy level？→ Level 1（robot assistance）。
3. Haptic feedback 和 motion boundary 屬於 passive support 還是 active guidance？→ Active guidance；tremor filtration 和 tool tracking 屬於 passive support。
4. 美國唯一的 open-platform 機器人廠商？→ THINK Surgical（TSolution-One、TMINI）。
5. 美國唯一的 active（Level 3）骨科機器人？→ TSolution-One。
6. 骨科第一台機器人是什麼？為什麼停產？→ ROBODOC（1992，THA 股骨 milling）；技術複雜、手術時間長、併發症多。
7. 手術機器人的直接成本大約多少？→ 40 萬–150 萬美元。
8. AR-THA 的 RCT 中，cup 落在 Lewinnek safe zone 的比例？→ 94% vs 64%，但臨床分數沒有差異。
9. 哪一種 AR 顯示方式在裝置故障時仍看得到術野？→ Holographic；pass-through 故障時會遮住視線。
10. 哪一種追蹤方式不需要視線、適合 IM nail interlocking？→ Electromagnetic tracking。
11. 為什麼戴 AR HMD 時常常不能用無菌手術頭盔？→ 面罩會擋住光學追蹤。
12. VR 手術訓練的主要限制？→ 缺乏觸覺回饋（ceiling effect），也難模擬少見解剖。

---

*本頁為兩版原文逐段比對後以中文自行整理的差異重點，非原文翻譯；數值以 OKU 15 原書為準。*
