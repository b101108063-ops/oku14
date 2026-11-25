---
title: "OKU 15 Ch.20: Application of Three-Dimensional Printing to Orthopaedic Surgery（OKU 14 CH19 更新）"
date: 2026-11-25
draft: false
tags: ["OKU15", "Translational Science", "3D Printing", "PSI", "版本差異"]
categories: ["OKU 15 更新"]
weight: 20
summary: "PDF 6 → 8 頁。範圍縮小為 3D printing 本身；OKU 14 的機器人、導航、術中 3D 影像（O-arm、Airo）、AR、bioprinting／4D printing 全部移出（機器人與導航見 OKU 15 [Ch.10]({{< relref "/oku15/chapter_10.md" >}})）。新增列印製程（powder bed fusion、G code、後處理）與大量臨床數字（足踝客製植入物、triflange、脊椎 cage、PSI、模型）。"
---

> **對照：**OKU 14 [CH19 Applications of Three-Dimensional Technologies in Orthopaedic Surgery]({{< relref "/chapter_19.md" >}}) → OKU 15 **Ch.20**｜PDF 6 → 8 頁｜作者：Samuel B. Adams Jr（足踝背景，單一作者）
>
> **來源說明：**掃描檔，本頁根據 OCR 文字整理。
>
> **閱讀方式：**🆕 新增；🔄 改變；✅ 一致；❌ OKU 15 不再涵蓋。
>
> 💡 **本版定位：**範圍**縮小為 3D printing 本身**；OKU 14 的機器人、導航、術中 3D 影像（O-arm、Airo）、AR、bioprinting／4D printing 全部移出（機器人與導航見 OKU 15 Ch.10）。新增**列印製程（powder bed fusion、G code、後處理）**與**大量臨床數字**（足踝客製植入物、triflange、脊椎 cage、PSI、模型）。

---

## 0. OKU 14 → 15 改版重點

| 面向 | OKU 14 Ch.19 | OKU 15 Ch.20 |
|---|---|---|
| 範圍 | 3D printing＋機器人＋導航＋術中 3D 影像＋AR＋bioprinting／4D | **只講 3D printing**：植入物、PSI、模型、orthotics／prosthetics |
| 製程 | CT → 3D 模型 → CAD → FEA | **Powder bed fusion（FDM、SLS）**、雷射或電子束、**segmentation → G code**、**postprocessing（annealing、stress relief、polishing、microblasting）** |
| 植入物 | 鈦、PEEK；Conformis、Zimmer Biomet；美國未核准 3D 列印 revision component | **足踝骨缺損 39 人 74% 免二次手術**、**talus osteonecrosis**、**custom TKA**、**triflange 17 篇 579 例 82.7% 存活、29% 併發症**、**脊椎 cage 98.9% 融合** |
| PSI | TKA 已確立、脊椎螺釘準確度↑ | **TKA 結果混合**；**THA 杯位可能較有益**（2024 MA）；複雜 revision 與畸形最有價值；脊椎快速採用 |
| 模型 | 教育、術前規劃 | **2022 RCT 脊椎骨折**、髖臼骨折預彎鋼板、**經驗不足者 >70% 改變計畫** |
| 新增 | — | **3D 列印 AFO、insole（扁平足）、上肢固定器** |
| 證據等級表 | 多數 Level IV、最高 III | 未列等級表；強調**無長期資料** |

---

## 1. 背景與優點

- 又稱 **additive manufacturing**：依數位模型**逐層堆疊**
- **1980 年代**首次描述；醫學／骨科應用始於 **2000 年代**
- 傳統 **subtractive**（銑削、鑄模）仍是多數植入物的製法；適合量產，但有廢料、需大型集中廠房與倉儲、前置時間長、難客製
- 3D printing：基材為**粉末、液體或線材**，廢料少
- **五大優點**（Key Study Point）：**極度彈性客製形狀、更複雜精細、免組裝步驟、減少廢料、減少庫存**
- 可做出傳統無法達成的設計：**內部互通孔隙（如 gyroid 結構）供骨長入**
- **骨科最常見的用途 = 完全客製的病人專屬植入物**

## 2. 列印流程

### 2.1 製程技術

| 用途 | 技術 |
|---|---|
| **金屬植入物（最常用）** | **Fused deposition modeling、selective laser sintering** → 皆屬 **powder bed fusion**：鋪一層 **鈦合金或 CoCr** 粉末 → **雷射或電子束**選擇性熔合 → 平台下降 → 再鋪粉 → 重複 |
| **Polymer（PSI、模型）** | **Material jetting、stereolithography** |

### 2.2 數位流程
1. **CT 或 MRI** 斷層影像（或 CAD 原創設計）
2. **Segmentation**：在軟體中把目標骨或骨折塊從周圍結構分離
3. 設計裝置（跨越缺損、對齊骨塊）
4. 設計檔 → 3D model file → **G code**（將 3D 模型轉為一系列 2D 層）
5. 列印
6. **Postprocessing**：**annealing、stress relief、polishing、microblasting、鑽孔、銑削** → 確保表面性質符合用途

> **Pitfall**：3D 列印植入物**不是印完就能用**，多數需要傳統加工的後處理。

## 3. 客製植入物

- 適應：**骨缺損、畸形、nonunion、primary 置換、複雜 revision、異常解剖、脊椎**
- 替代：allograft、**vascularized bone graft**、現成金屬植入物、**Masquelet**、**bone transport**（各有 nonunion、感染、再手術等問題）

### 3.1 足踝

| 研究 | 結果 |
|---|---|
| 2022，**39 人**，足踝 critical bone loss | 平均 27 個月，**74% 不需第二次手術** |
| **15 人**，嚴重骨缺損／畸形矯正／融合 | **僅 2 例失敗** |
| 2025，**talus osteonecrosis** | 可精確重建個人解剖、**恢復 talar height 與 tilt、保留周圍關節活動** |
| 2025，**38 人** | 2 年時足踝放射學對位與功能顯著改善 |

- 課本病例：槍傷無法重建的 navicular → **鈦製 navicular 替代物**（螺孔、tab、gyroid 內部結構）

### 3.2 關節置換
- **現成植入物仍是 standard of care**；客製可能是安全替代
- **Custom TKA**：脛骨元件 **fit 與 rotation 改善**、不良事件↓、**成本節省**（各一篇研究）
- **Revision THA 嚴重髖臼骨缺損 → custom triflange**（可最大化骨接觸）
  - **MA：17 篇、579 例 → revision-free survivorship 82.7%、併發症 29%**，術後髖分數改善

### 3.3 孔隙與骨長入
- 增加孔隙 → 骨長入、**更接近原生骨力學性質**、血管化與細胞浸潤
- **脊椎：93 人，3D 列印 lamellar titanium cage＋植骨 → 1 年融合率 98.9%**

## 4. Patient-Specific Instrumentation（PSI）

- 可搭配 3D 列印或現成植入物；目標：提升截骨、植入物位置與對位的準確度
- **TKA：手術時間與對位的結果混合**
- **THA：髖臼杯位與尺寸需精確 → PSI 可能更有益**（anteversion、abduction 角度符合解剖）
  - **2024 MA**：**術前杯尺寸規劃準確度↑、術後 Harris Hip Score↑**
  - 小型 RCT：**手術時間↓、成本↑**
  - 另一研究：**時間更長、更貴、結果無差**
- **最有價值：複雜 revision 與畸形**（術前規劃矯正截骨、異常解剖）
- **脊椎**：每節客製 drill guide 已相對普及；早期結果佳，需長期追蹤
- 課本病例：**Charcot 遠端脛骨切骨導板**

> OKU 14 說「PSI 在 TKA 已有明確證據」；**OKU 15 改為 TKA 結果混合、THA 與複雜病例較有潛力**。

## 5. 解剖模型

- 術前規劃、術中參考、教學；比 2D 或斷層影像提供更完整資訊
- **2022 RCT（脊椎骨折）**：術中有 3D 模型 → **手術時間、失血、透視顯著↓**；螺釘位置改善不顯著
- **髖臼骨折**：依模型**術前預彎鋼板** → 失血與手術時間↓、復位改善
- 鎖骨、肩胛骨骨折也有類似好處
- **>100 位骨科醫師選擇複雜脛骨骨折鋼板**：
  - **經驗不足者（<15 例類似骨折）看過模型後 >70% 改變計畫**
  - 有經驗者較少改變，但 **>70% 支持在臨床使用**
  - → **模型效益可能隨經驗增加而遞減**
- 教育：病人、醫學生、住院醫師、主治醫師；無風險環境練習技術

## 6. 客製 Orthotics 與 Prosthetics

- 傳統 AFO 需**石膏取模**：耗工、易誤差、貼合與舒適度問題
- 3D 列印依醫學影像或**體表 3D 掃描**製作 → 流程簡化
- **3D 列印鞋墊 > 預製鞋墊（症狀性扁平足）**
- **3D 列印上肢固定器 vs fiberglass cast → 舒適、功能、滿意度更高**

## 7. 總結

- 早中期結果在多個次專科都有前景
- **沒有長期資料**——臨床應用仍相對新
- 獨特之處：短時間、合理成本內做出客製內外部結構

---

## 8. 陷阱與易混淆

1. 金屬 3D 列印植入物的主要製程是 **powder bed fusion**（雷射或電子束熔合鈦合金／CoCr 粉末）；polymer 用 material jetting 或 stereolithography
2. **Segmentation → G code** 的順序；印完要 **postprocessing**
3. 骨科 3D 列印**最常見用途 = 客製植入物**（不是模型）
4. **Triflange：82.7% 存活、但併發症 29%**
5. **脊椎 3D 列印鈦 cage 融合率 98.9%**
6. **PSI 在 TKA 證據混合**；在 THA 杯位、複雜 revision、畸形較有價值
7. 模型的效益**對經驗不足者最大**（>70% 改變計畫）
8. 現成植入物仍是 primary 置換的 standard of care
9. OKU 14 的機器人、導航、O-arm、AR、4D printing **不在本章**

---

## 9. Key Study Points（OKU 15）

- 3D printing 優點：極度彈性客製形狀、更精細複雜、免組裝、減少廢料、減少庫存
- 3D 列印客製植入物已用於骨缺損、畸形、nonunion、primary 置換、複雜 revision、異常解剖、脊椎
- 術前使用 3D 列印解剖模型可減少手術時間、失血，並**在經驗不足的醫師手中改善骨折復位**

---

## 10. Anki 候選題

1. 金屬植入物最常用的兩種列印技術屬於哪一類製程？使用哪些金屬？ → Powder bed fusion（FDM、SLS）；鈦合金、cobalt-chromium
2. 從 CT 到列印的數位流程中，哪一步把結構從周圍組織分離？哪一步把 3D 模型轉成 2D 層？ → Segmentation；G code
3. Custom triflange 的 MA 存活率與併發症率？ → 82.7% revision-free survivorship；29% 併發症
4. PSI 在 TKA 與 THA 的證據有何差異？ → TKA 結果混合；THA 杯位與尺寸規劃準確度與 HHS 改善（2024 MA），但成本與時間結果不一
5. 3D 模型對哪類醫師的影響最大？數字為何？ → 經驗不足者（<15 例）；>70% 看過模型後改變計畫

---

*本頁為 OKU 15 原文（OCR）與 OKU 14 筆記逐段比對後，以中文自行整理的差異重點，非原文翻譯；數值以原書為準。*
