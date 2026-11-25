---
title: "OKU 15 Ch.14: Biomaterials and Implants: Regenerative Engineering Approaches for Orthopaedics（OKU 14 CH13 更新）"
date: 2026-11-25
draft: false
tags: ["OKU15", "Translational Science", "Biomaterials", "Regenerative Engineering", "版本差異"]
categories: ["OKU 15 更新"]
weight: 14
summary: "PDF 12 → 8 頁。篇幅縮短（8 頁），從「electrospinning 物理與 3D/4D/5D 列印」轉為「MSC＋三大生長因子＋四類 scaffold 材料＋三種製程＋各組織應用」的入門架構。"
---

> **對照：**OKU 14 [CH13 Biomaterials and Implants]({{< relref "/chapter_13.md" >}}) → OKU 15 **Ch.14**｜PDF 12 → 8 頁｜作者：Gregory R. Roytman, Johannes M. Sieberer, Steven M. Tommasini, Daniel H. Wiznia（作者群全換）
>
> **來源說明：**掃描檔，本頁根據 OCR 文字整理。
>
> **閱讀方式：**🆕 新增；🔄 改變；✅ 一致；❌ OKU 15 不再涵蓋。
>
> 💡 **本版定位：**篇幅縮短（8 頁），從「electrospinning 物理與 3D/4D/5D 列印」轉為「**MSC＋三大生長因子＋四類 scaffold 材料＋三種製程＋各組織應用**」的入門架構。

---

## 0. OKU 14 → 15 改版重點

| 面向 | OKU 14 Ch.13 | OKU 15 Ch.14 |
|---|---|---|
| 架構 | Top-down／bottom-up 典範、scaffold 三性質、electrospinning 不穩定性、3D/4D/5D printing | 幹細胞與生長因子 → scaffold 材料（polymer、hydrogel、ceramic、metal）→ 製程（electrospinning、**microfluidics**、3D printing）→ 骨／軟骨／韌帶肌腱 |
| 新增 | — | **BMP／TGF-β／IGF-1 三大生長因子家族**、MSC 來源比較、scaffold 力學名詞（modulus、strength、**creep**）、**metal stress shielding**、**microfluidics（organ-on-a-chip）**、ARMI、2023 phase 3 MSC 膝 OA 試驗、allogeneic MSC 引發後天免疫 |
| 刪除 | Electrospinning Rayleigh／whipping 不穩定性、modulus 決定 chondro vs osteo 分化（PES-PCL 研究）、4D／5D printing、printed acetabulum retrieval study、YAP/TAZ viscosity | 3D printing 臨床應用移至 [Ch.20]({{< relref "/oku15/chapter_20.md" >}}) |

---

## 1. 背景

- Regenerative medicine 早期：**prolotherapy**（刻意誘發細胞死亡 → 發炎 → 修復），至今在肌肉骨骼醫學仍最常用
- 第一批幹細胞約 50 年前描述；約 20 年前證實可「程式化」分化 → 領域爆發
- 現代三要素：**progenitor cell ＋ growth factor ＋ extracellular structure（scaffold）**；ECM 的方向、結構、應力應變與材料決定分化
- **ARMI（Advanced Regenerative Manufacturing Institute）**：New Hampshire 的公私合作非營利機構，約 200 個產學成員，推動材料、檢測、細胞株標準化

## 2. 幹細胞

- **所有肌肉骨骼細胞源自 MSC**；MSC 來自胚胎 **mesoderm**，於**第 3 週 gastrulation** 開始發育
- 成人 MSC 來源：**adipose、bone marrow、synovium、umbilical cord blood**、周邊血、胎兒組織（後者有爭議）
- **Bone marrow MSC = 最常用**（易取得、易採集、存活率高），且**軟骨分化能力較佳**

## 3. 三大生長因子家族（高頻考點）

| 家族 | 重點 |
|---|---|
| **BMP** | 成骨主要為 **BMP-2、4、6、7、9**；BMP-2 → osteoblast 分化；BMP-4 → 骨折修復；**BMP-2、4 同時活化 osteoclast** → rhBMP 臨床結果參差；臨床前研究：合併 **bisphosphonate** 抑制 osteoclast 可增強成骨；**BMP-9 = 軟骨生成因子**（機轉爭議：ECM 沉積 vs 非等向排列） |
| **TGF-β** | 幾乎所有肌肉骨骼組織發育；經 latent TGF-β binding protein 結合 **hydroxyapatite**；**TGF-β1**：ECM 重塑、**ACL 癒合**、纖維母細胞膠原沉積；TGF-β1 ＋ BMP-2 協同 → 軟骨生成；**TGF-β3**：軟骨生成，2023 研究用於 **rotator cuff 軟骨–肌腱交界修復** |
| **IGF-1** | osteoblast、chondroblast 分化；啟動 **mTOR**；經 **IGF-1R → MAPK–ERK1/2** 促 MSC 增殖遷移；軟骨再生；**肌腱再生能力 ≥ BMP、TGF-β** |

> **Pearl**：「BMP 既促成骨也促破骨」是解釋 rhBMP-2 臨床不一致（含骨溶解、血清腫）的核心觀念。

## 4. Scaffold 設計

**力學名詞**
- **Stiffness = Young（elastic）modulus**：受應力時的變形程度
- **Strength**：降伏或斷裂時的力／應力
- **Creep**：持續應力下隨時間發生的塑性變形，最終失效 → 每日反覆負荷的肌肉骨骼組織需考慮
- **Biocompatibility = 最重要**：非發炎、血液相容、無毒、非過敏、非致癌
- **Conductive properties**：讓血管與周圍組織長入、整合移植物

### 4.1 四類材料

| 類別 | 代表 | 優點 | 缺點／重點 |
|---|---|---|---|
| **合成 polymer** | PCL、PLA、PGA、**PLGA**（常用共聚物） | 易控制、易合成；長期植入 scaffold | 均一性不適合特殊幾何；生物相容性可能差 |
| | **PMMA** | 骨水泥、骨替代物 | 硬且脆，其他用途受限 |
| **天然 polymer** | **Collagen**（所有肌肉骨骼）、**hyaluronic acid**（軟骨、筋膜）、**silk fibroin**（韌帶、骨、軟骨、血管）、**chitin**（甲殼，無毒可分解強度高）、**PHA**（細菌合成 polyester） | 生物相容性佳 | 力學差；PHA 具 **piezoelectricity** → 傷口癒合 |
| **Hydrogel** | 保水 polymer 基底 | **軟骨再生**理想；可分解、黏附，讓原生細胞移入；**smart hydrogel** 可對化學／電／機械刺激改變性質 | 3D bioprinting 主要的 **bioink** |
| **Ceramic** | **Bioinert**（THA bearing）、**Bioactive**（calcium phosphate，最常用 **hydroxyapatite**） | Bioinert：耐腐蝕、低磨耗、少磨屑；HA：無毒、親水、成分近骨與牙 | **HA 本身力學弱** → 複合材料、奈米技術、3D 列印、雷射燒結 |
| **Metal** | 鋼板、髓內釘、螺絲；trabecular metal | 生物相容、免疫反應小、力學佳、製程成熟 | 磨耗／腐蝕釋出金屬顆粒；**modulus 遠高於宿主 → stress shielding**（對 MSC 分化不利）→ 多改作複合材料的結構元件或 coating |

- 骨工程 scaffold 三類：合成（力學好、惰性、親水與黏附差）、天然（相容好、力學差）、**複合**（兩者兼得）
- **PCL 已獲 FDA 核准臨床使用**（尤其顱顏骨修復）；問題：**降解慢、生物活性低**

## 5. 製程

| 製程 | 原理 | 重點 |
|---|---|---|
| **Electrospinning** | 帶電溶液擠入電場 → 收集板沉積、溶劑揮發成支架 | 準確、易用、可控 → 最廣用；新進展：改配方、纖維排列模仿奈米幾何、**加入顯影劑（radiopaque）追蹤癒合**；短期內不會被淘汰 |
| **Microfluidics（新）** | **Organ-on-a-chip**；微流道導入奈米級流體模擬器官環境 | 優於靜態 bioreactor：可產生**複雜湍流傳遞機械訊號**；已能模擬胚胎分化環境並整合多種組織 |
| **3D printing／bioprinting** | 積層製造；bioprinting = 為生物用途列印、可種細胞的結構 | 優點：形狀結構控制度高；缺點：難以原生組織列印；**bioink 多為 hydrogel**；可無細胞、含細胞或分區封裝細胞；**限制：解析度、需黏稠 bioink 才能擠出 → 難印高剛性材料** |

## 6. 各組織應用

### 6.1 骨
- 大缺損無法自癒 → autograft、allograft、xenograft（感染、取得量、排斥風險）
- **Allogeneic MSC 注射可改善 OI 癒合**，無不良反應
- **2023 phase 3 RCT**（隨機、雙盲、多中心、安慰劑對照）：商業 MSC 產品治療**膝 OA** 有效且安全
- 動物研究：**重複關節內注射 allogeneic MSC → 後天免疫反應**（autologous 無）→ 需謹慎
- **MSC 單獨無法橋接大骨缺損** → 理想 scaffold 四條件：
  1. 優異生物相容性（黏附、增殖、引導分化）
  2. **降解速率 ≈ 骨再生速率**
  3. 允許活組織代謝
  4. 滿足初期力學穩定（下肢尤其高）

### 6.2 軟骨
- 晚期 OA 目前除 **TJA** 外無高效治療
- **MACI = 美國已註冊的細胞產品**（課本稱 MSC-based）
- 障礙：關節內**發炎環境**與活動負荷
- **Scaffold-free 方法**：無 stress shielding、更接近原生軟骨，但依賴困難的自組裝

### 6.3 韌帶與肌腱
- 現行：allograft、autograft、xenograft、人工移植物
- 挑戰：scaffold 需支持 MSC 黏附分化，**同時在完全降解前具備足夠彈性與強度**
- 動物研究有早期成果，**尚無人體應用報告**

---

## 7. 陷阱與易混淆

1. **BMP-9 是軟骨生成因子**，不是典型成骨用的 BMP-2/7
2. **BMP-2 與 BMP-4 也會活化 osteoclast**
3. **TGF-β3（軟骨、rotator cuff 交界）vs TGF-β1（ACL 癒合、膠原沉積）**
4. 金屬問題的關鍵字是 **stress shielding（modulus 過高）**，不是生物相容性差
5. HA ceramic 是 bioactive 但**本身力學弱**；bioinert ceramic 才用於 bearing surface
6. Bone marrow MSC 最常用；adipose MSC 單位體積產量高（見 [Ch.17]({{< relref "/oku15/chapter_17.md" >}})）
7. Allogeneic MSC **重複注射**可能引發後天免疫
8. Bioprinting 限制在**黏度與解析度**，不是材料成本

---

## 8. Key Study Points（OKU 15）

- MSC 是肌肉骨骼細胞系的基礎，其分化受多種生長因子影響
- 再生組織的生物製造受限於擠出所需的原料**黏度**，尤其當目標組織需要較高剛性時
- 細胞、生長因子與 scaffold 幾何需依解剖部位與個別病人量身調整

---

## 9. Anki 候選題

1. 成骨相關的 BMP 有哪些？哪一個是軟骨生成因子？ → BMP-2、4、6、7、9；BMP-9
2. 為何 rhBMP 臨床結果不一致？臨床前有何對策？ → BMP-2／4 同時活化 osteoclast；合併 bisphosphonate
3. 金屬作為再生 scaffold 的主要力學缺點是什麼？ → Young modulus 遠高於宿主組織 → stress shielding
4. 理想骨 scaffold 的四個條件？ → 生物相容（黏附、增殖、引導分化）、降解速率配合骨再生、允許代謝、初期力學穩定
5. Microfluidics 相對靜態 bioreactor 的優勢？ → 可產生複雜湍流傳遞機械訊號，模擬器官／胚胎環境
6. 哪一種 polymer 已獲 FDA 核准用於骨修復 scaffold？缺點是什麼？ → PCL；降解慢、生物活性低

---

*本頁為 OKU 15 原文（OCR）與 OKU 14 筆記逐段比對後，以中文自行整理的差異重點，非原文翻譯；數值以原書為準。*
