---
title: "OKU 15 Ch.7: Musculoskeletal Biomechanics and Biomaterials（OKU 14 CH8 更新）"
date: 2026-11-25
draft: false
tags: ["OKU15", "General Topics", "Biomechanics", "Biomaterials", "版本差異"]
categories: ["OKU 15 更新"]
weight: 7
summary: "篇幅 8 → 14 頁，單一作者重寫。寫法改成通論式、數字很少。新增剛體力學與關節自由度、疲勞分析、骨折癒合四期、各類生物材料（含 PLA／PGA、CFRP、bioactive glass、天然材料）、UHMWPE 交聯與 vitamin E、3D 列印。OKU 14 的彎曲試驗、load vs displacement control、腐蝕機轉（pitting、crevice、MACC）、鋯與鉭等不再涵蓋。"
---

> **對照：**OKU 14 [CH8 Musculoskeletal Biomechanics and Biomaterials]({{< relref "/chapter_08.md" >}}) → OKU 15 **Ch.7**（同名）｜PDF 8 → 14 頁（+75%）｜單一作者重寫
>
> **來源說明：**掃描檔，本頁根據 OCR 文字整理。
>
> **閱讀方式：**🆕 新增；🔄 改變；✅ 一致；❌ OKU 15 不再涵蓋。
>
> 💡 **讀法建議：**OKU 15 這章篇幅變長，但寫成通論式，**很少有具體數值**。OKU 14 CH8 的彈性模數比較、腐蝕機轉、合金特性仍是材料題的主要考點，**請以 OKU 14 筆記為主，本頁當作補充**。

## 0. 考點變更總表

| 主題 | OKU 14 CH8 | OKU 15 Ch.7 | 類型 |
|---|---|---|---|
| 寫法 | 數據導向：載荷模式、三種彎曲試驗、應力應變曲線、模數比較 | **通論式**，以定義為主，幾乎沒有數字 | 🔄 |
| 剛體力學與關節運動學 | — | 🆕 Free-body diagram、平衡、**6 個自由度**、各類關節的自由度 | 🆕 |
| 應力應變曲線 | Yield、UTS、塑性變形 | 🔄 改為分類：linear elastic、elastic-plastic、nonlinear elastic、hardening 與 softening、viscoelastic | 🔄 |
| 黏彈性 | 遲滯、應力鬆弛、蠕變 | ✅ 相同；加上 **strain rate sensitivity**（骨頭承受快速負荷的能力較好） | ✅ |
| 等向性 | — | 🆕 Isotropic（金屬）vs **anisotropic（骨頭）** | 🆕 |
| 疲勞 | 疲勞特性 | 🔄 加上 **fatigue life** 與植入物疲勞分析的流程 | 🔄 |
| 實驗測試方法（load vs displacement control） | 有 | **不再涵蓋**；只提到 in vitro、in vivo、in silico 測試 | ❌ |
| 骨折癒合與固定 | — | 🆕 **四期**（發炎、軟骨痂、硬骨痂、重塑）＋固定的力學併發症 | 🆕 |
| 生物材料特性與生物相容性 | 骨、PE、PMMA、合金 | 🆕 一長串特性定義；生物相容性的**四種交互作用** | 🆕 |
| 金屬 | 不鏽鋼、CoCr、Ti 的模數與特性；**鋯與鉭** | 🔄 三種金屬的優缺點與失效機轉；**鋯與鉭不再涵蓋** | 🔄 |
| 陶瓷 | 有 | 🔄 alumina、**Biolox delta**、zirconia、calcium phosphate | 🔄 |
| UHMWPE | 有 | 🆕 **交聯方法**（gamma、e-beam、UV）、**vitamin E**、**calcium stearate 已停用** | 🆕 |
| 其他高分子與複合材料 | — | 🆕 **PLA／PGA**（可吸收）、**CFRP**（放射線可穿透）、**bioactive glass** | 🆕 |
| 天然材料 | — | 🆕 Collagen、chitosan、silk | 🆕 |
| 3D 列印 | — | 🆕 多孔結構、病人專屬設計 | 🆕 |
| 腐蝕（三步驟、鈍化膜、**pitting、crevice、MACC**） | 獨立一節 | **不再涵蓋**，只零星提到腐蝕與離子釋出 | ❌ |

---

## 1. 剛體力學與關節運動學 🆕
- **剛體力學**：研究受外力時**不會變形**的物體的運動與平衡。骨頭在生理負荷下變形很小，常被當作剛體分析。
  - **平衡** = 所有力與力矩的總和為零（靜止或等速運動）。
  - **Free-body diagram**：畫出作用在物體上的所有外力與力矩，用來推算骨頭或植入物內部的力。
- **關節運動學**：人體關節**最多有 6 個自由度**，即 **3 個平移加 3 個旋轉**。

| 關節類型 | 例子 | 自由度 |
|---|---|---|
| Hinge | **肘、膝**（簡化模型） | **1**（屈伸） |
| Ball-and-socket | **肩、髖** | **3**（屈伸、外展內收、內外旋） |
| Pivot | **近端 radioulnar joint** | **1**（旋前旋後） |

> 膝關節完整描述其實需要 6 個自由度：3 個平移（前後、內外、上下）與 3 個旋轉（屈伸、內外翻、軸向旋轉）。原書附圖就是用膝關節示範 6 個自由度。

## 2. 可變形材料 🔄

### 2.1 基本定義
- **力**的單位是 N。**應力 = 單位面積的內力**（Pa 或 MPa）；**應變 = 相對長度或角度的變化**（沒有單位）。
- **Young modulus（彈性模數）** = 線性彈性區的應力 ÷ 應變，代表**剛度（stiffness）**。
- **Elastic limit**：不產生永久變形所能承受的最大應力。

### 2.2 應力應變曲線的類型
| 類型 | 曲線特徵 |
|---|---|
| Linear elastic | 通過原點的直線，斜率就是 Young modulus |
| Elastic-plastic | 彈性段之後，從 **yield point** 開始進入塑性段；塑性段的斜率稱為 plastic modulus |
| Nonlinear elastic | 曲線，剛度以 **tangent modulus**（某點的切線斜率）表示 |
| Hardening／softening | 塑性段斜率遞增（愈變形愈硬）或遞減 |
| Viscoelastic | **曲線形狀取決於負荷速度與負荷歷程** |

### 2.3 黏彈性 ✅
- **Creep**：定應力下應變隨時間增加。
- **Stress relaxation**：定應變下應力隨時間下降（例如拉住的橡皮筋）。
- **Hysteresis**：反覆加載與卸載時，曲線形成迴圈，能量以熱的形式損失。
- 🆕 **Strain rate sensitivity**：**骨頭承受快速負荷的能力比緩慢負荷好**，例如跑步這類高衝擊活動，骨頭能吸收較多能量。

### 2.4 等向性 🆕
- **Isotropic**：各方向性質相同，例如鋼、鋁等金屬。
- **Anisotropic**：性質隨負荷方向改變，**骨頭是典型例子**。原因是膠原纖維、礦物晶體與細胞成分以不同方向排列的階層結構。

### 2.5 疲勞 🔄
- **疲勞**：反覆負荷造成漸進、局部的結構損傷，**即使應力低於 UTS 也可能失效**。
- **Fatigue life**：材料或結構在失效前能承受的循環次數。影響因素包括材料、負荷大小與頻率、幾何形狀、**表面處理**，以及**應力集中或缺陷**。
- 植入物疲勞分析的步驟：了解負荷與體內環境 → 量測材料的疲勞強度 → 用電腦模擬找出可能失效的部位 → 改進設計、材料或表面處理。

## 3. 生物組織的力學性質與測試 🆕
- 組織的力學性質取決於**結構、組成、含水量、溫度與負荷速度**。
- 特性定義：stiffness（抵抗變形）、strength（失效前的最大應力）、elasticity、plasticity、viscoelasticity、anisotropy（隨方向變化）、**heterogeneity（隨位置變化）**、nonlinearity。
- 測試可以是 **in vitro、in vivo 或 in silico**。
- 骨與關節的應力應變分析方法：beam theory、continuum mechanics、finite element analysis、multibody dynamics。

## 4. 骨折癒合與固定的力學 🆕
- **癒合四期：**
  1. **Inflammation**：出血、凝血、發炎、疼痛
  2. **Soft callus**：纖維母細胞、軟骨細胞與血管形成軟組織橋接
  3. **Hard callus**：woven bone 與軟骨取代軟骨痂
  4. **Remodeling**：移除多餘骨質，形成 lamellar bone
- 骨折部位的**力學環境**（負荷的大小、方向、頻率、持續時間）會影響癒合的速度與品質；力學刺激會調控細胞的增生、分化、遷移與基質合成。
- **固定方式**依位置分為 **external** 與 **internal fixation**。效能取決於器材的設計、材料與配置，以及骨質與幾何。
- **力學併發症**：植入物鬆脫、斷裂、感染、nonunion、malunion、delayed union。

## 5. 生物材料 🔄

### 5.1 生物相容性 🆕
- **定義：材料能發揮預期功能，且不引起不良的生物反應。**
- 相關概念：**bioactivity**（誘發特定生物反應）、**bioresorbability**（可被分解吸收）、bioadhesion、**biointegration**（與組織形成穩定的介面）。
- **材料與生物系統的四種交互作用：physical**（熱、電、輻射）、**chemical**（腐蝕、降解、藥物釋放）、**biologic**（發炎、感染、整合）、**mechanical**（應力、應變、壓力的傳遞）。
- **Tribology** = 研究互相接觸表面的摩擦、磨損與潤滑。

### 5.2 金屬 🔄

| 金屬 | 用途 | 優點 | 缺點與失效機轉 |
|---|---|---|---|
| **不鏽鋼** | **暫時性植入物**：骨板、螺釘、髓內釘 | 強度高、延展性好、便宜、容易加工 | 長期會**腐蝕**，釋出 **nickel、chromium** 離子（過敏、組織刺激）；密度高、較重；**osseointegration 不如鈦**。所以**不用於永久植入物** |
| **鈦與鈦合金** | **永久植入物**：關節置換、脊椎植入物 | 生物相容性佳（**穩定的氧化層**可防腐蝕並促進細胞附著）、抗疲勞、抗腐蝕、**強度重量比高**、表面可改質以促進 osseointegration | **Notch sensitivity**：表面瑕疵會明顯降低疲勞強度，裂縫由此產生；**硬度低於 CoCr**，用在承重關節面會磨損並產生 osteolysis；較貴 |
| **CoCr 合金** | **關節置換的承重面**、脊椎 rod、骨折固定 | **耐磨、強度高**、抗腐蝕 | **金屬離子釋出**（Co、Cr）造成發炎、**metallosis**、過敏；**模數高，造成 stress shielding** |

> **骨板比較題：**不鏽鋼骨板主要的失效機轉是長期腐蝕，加上 notch sensitivity 造成應力集中與微裂縫；鈦骨板較不易腐蝕，失效主要來自 **notch sensitivity 造成的應力集中**。

### 5.3 陶瓷 🔄
- 優點：**硬度高、耐磨、低摩擦、抗化學腐蝕**、生物相容性好。
- 缺點：**脆**，在高應力或衝擊下可能**突然碎裂**，碎片很銳利，需要翻修；製程要求精密（不能有微裂縫），成本高；**模數高**，應力分散較差。抗壓強度高，但**怕張應力**。
- **Alumina**：用於 THA 的 ceramic 股骨頭搭配 PE 襯墊，比 metal-on-PE 磨屑少。**Biolox delta** 是性能更好的改良型。
- **Zirconia**：**強度與韌性比其他陶瓷高**，較不易碎裂，用於髖與膝的承重面。
- **Calcium phosphate（hydroxyapatite、TCP）**：具 **osteoconductive** 性質，用作骨移植替代物與金屬植入物的塗層。

### 5.4 高分子 🆕
- **UHMWPE**：自 **1960 年代**起用於關節置換。
  - 主要問題是**磨屑引起的 osteolysis**：PE 顆粒活化 macrophage 與 osteoclast，造成植入物周圍骨吸收、鬆脫。
  - **交聯（cross-linking）**：以輻射在高分子鏈之間形成共價鍵，**大幅提高耐磨性**。方法有三種：
    - **Gamma 輻射**（cobalt-60）：穿透深且均勻，最常用
    - **Electron beam**：劑量與深度控制精確
    - **UV**：較少用，可以只處理表面
  - 交聯的代價：**疲勞強度與抗拉強度下降**。
  - **Vitamin E**：抗氧化劑，可以防止氧化降解，又不犧牲機械性質。
  - **Calcium stearate**（成核劑）：**會增加磨損，已停用**。
- **PMMA（骨水泥）**：在原位硬化，提供即時固定，也用來填補骨缺損或當 spacer。
- **PLA／PGA**：**可吸收**，用於縫線、螺釘、骨板，分解成乳酸與甘醇酸後被代謝，**不需要再手術取出**。

### 5.5 複合材料與天然材料 🆕
- **CFRP（carbon fiber-reinforced polymer）**：強度重量比高，而且**放射線可穿透**，術後影像追蹤比較清楚，用於骨折固定。
- **Bioactive glass**：釋出離子刺激細胞，促進 hydroxyapatite 形成並**與骨頭鍵結**，用於骨移植與 scaffold。
- **Collagen**（scaffold、敷料，可加生長因子）、**chitosan**（取自 chitin，**具抗菌性**，可做成膜、凝膠或海綿）、**silk**（縫線、scaffold，強度高且可緩慢分解）。

### 5.6 植入物的種類與選擇
- 類別：關節置換、骨折固定、脊椎植入物、骨移植與替代物、軟骨修復、韌帶與肌腱重建、orthobiologics、支架與義肢。
- 選擇時要考量的因素：臨床問題、病人特性、材料性質、幾何、固定方式、效能、耐久性、相容性、成本、可取得性。

### 5.7 3D 列印 🆕
- 可以做出**傳統製造做不到的複雜幾何與病人專屬設計**，改善貼合度與功能。
- **多孔結構可以模擬骨頭的天然結構，促進 osseointegration**，提升穩定度與壽命。
- 可使用鈦合金、bioactive ceramics 等材料，並調整力學與生物特性。

---

## 6. OKU 14 CH8 中 OKU 15 不再涵蓋的內容 ❌（材料題重點，請保留 OKU 14 筆記）
- **載荷模式與三種彎曲試驗**（3-point、4-point、cantilever）
- **Yield point、UTS、塑性變形的數值意義**
- **各材料彈性模數的比較**（皮質骨、松質骨、Ti、CoCr、不鏽鋼、PE、PMMA、陶瓷）
- **Load control vs displacement control**
- **皮質骨與松質骨的力學性質**
- **PMMA 的細節**（聚合放熱、抗壓強但抗拉弱等）
- **鋯（oxinium）與鉭（trabecular metal）**
- **腐蝕：驅動力與三步驟、鈍化膜、pitting、crevice、MACC（mechanically assisted crevice corrosion）**

> 這些都是 OKU 與專科考試的傳統高頻題，尤其是**模數排序**和 **MACC（taper corrosion）**。

---

## 7. Anki 候選題

1. 人體關節最多有幾個自由度？→ 6 個（3 個平移、3 個旋轉）。
2. 肩與髖、肘與膝（簡化模型）、近端 radioulnar joint 各有幾個自由度？→ 3；1；1。
3. Young modulus 的定義？→ 線性彈性區應力 ÷ 應變，代表剛度。
4. Stress relaxation 和 creep 的差別？→ Stress relaxation 是定應變下應力下降；creep 是定應力下應變增加。
5. 骨頭承受快速負荷還是緩慢負荷的能力較好？→ 快速負荷（strain rate sensitivity）。
6. 為什麼骨頭屬於 anisotropic 材料？→ 膠原、礦物與細胞以不同方向排列，性質隨負荷方向改變。
7. 骨折癒合的四期？→ Inflammation、soft callus、hard callus、remodeling。
8. 為什麼不鏽鋼不用於永久植入物？→ 長期腐蝕會釋出 Ni、Cr 離子，較重，osseointegration 較差。
9. 鈦合金最大的力學弱點？→ Notch sensitivity；另外硬度低，不適合當承重面。
10. CoCr 合金的主要缺點？→ 金屬離子釋出（metallosis、過敏），以及模數高造成 stress shielding。
11. 陶瓷承重面最大的風險？→ 脆、突然碎裂；怕張應力。
12. 哪一種陶瓷的韌性比其他陶瓷高？→ Zirconia。
13. UHMWPE 的三種交聯方法？交聯的代價？→ Gamma、electron beam、UV；疲勞強度與抗拉強度下降。
14. 哪一種添加物可以防止 PE 氧化，又不影響機械性質？哪一種因為增加磨損而停用？→ Vitamin E；calcium stearate。
15. 哪一種複合材料的優點是放射線可穿透？→ CFRP。
16. PLA／PGA 植入物的優點？→ 可吸收，不需要再手術取出。

---

*本頁為 OKU 15 原文（OCR）與 OKU 14 筆記逐段比對後，以中文自行整理的差異重點，非原文翻譯；數值以原書為準。*
