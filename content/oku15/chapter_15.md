---
title: "OKU 15 Ch.15: Musculoskeletal Mechanics and Kinesiology（OKU 14 CH14 更新）"
date: 2026-11-25
draft: false
tags: ["OKU15", "Translational Science", "Biomechanics", "Kinesiology", "版本差異"]
categories: ["OKU 15 更新"]
weight: 15
summary: "PDF 14 → 16 頁。加強基礎力學與骨材料測試（Newton 三定律、load–displacement 四參數、material vs structural property、cartilage biphasic），動作分析改為光學／IMU／markerless／wearable／EMG／OpenSim／FEA 的技術比較；OKU 14 的髖膝步態運動學、接觸力表與 DFIS 臨床結果大幅刪除。"
---

> **對照：**OKU 14 [CH14 Musculoskeletal Mechanics and Kinesiology]({{< relref "/chapter_14.md" >}}) → OKU 15 **Ch.15**｜PDF 14 → 16 頁｜作者：Steven M. Tommasini, Aidin Eslam Pour
>
> **來源說明：**掃描檔，本頁根據 OCR 文字整理。
>
> **閱讀方式：**🆕 新增；🔄 改變；✅ 一致；❌ OKU 15 不再涵蓋。
>
> 💡 **本版定位：**加強**基礎力學與骨材料測試**（Newton 三定律、load–displacement 四參數、material vs structural property、cartilage biphasic），動作分析改為**光學／IMU／markerless／wearable／EMG／OpenSim／FEA** 的技術比較；OKU 14 的髖膝步態運動學、接觸力表與 DFIS 臨床結果大幅刪除。

---

## 0. OKU 14 → 15 改版重點

| 面向 | OKU 14 Ch.14 | OKU 15 Ch.15 |
|---|---|---|
| 新增 | — | Newton 三定律、torque = F×d、**whole-bone 四參數**（stiffness、max load、displacement、work-to-fracture）、**material（intrinsic）vs structural（extrinsic）**、「骨為何斷」（能量吸收）、**cartilage biphasic indentation（H_A、ν、k）**、三種軟骨、**IMU drift**、**markerless（深度＋RGB＋ML）**、smart shoe、surface vs intramuscular EMG、**OpenSim Gait2392**、**FEA** |
| 數字變動 | 骨：HA 40%、collagen 35%、水 25% | 骨：**mineral 約 65%、organic 35%**（＋細胞、水）；organic 中 **collagen 90%、NCP 10%** |
| | 動作捕捉相機 **5–10 台** | **8–16 台** |
| 刪除 | 髖膝 6 DOF 步態角度、髖接觸力表（Bergmann／Paul）、膝滾動滑動「8」字路徑、DFIS 精度（<0.9 mm／<0.6°、5–6 mSv）與 TKA／THA 運動學結果、可穿戴效度差 25% | Dual fluoroscopy 只剩一段（輻射、12 吋 image intensifier 限制） |

> **考試提醒**：OKU 14 的步態角度、髖接觸力倍數、DFIS 精度仍是常見題目來源；本版不再列出，兩版要並讀。

---

## 1. 基礎力學

- **Newton 三定律**：(1) 慣性定律（uniform motion）(2) **F = ma**（F 與 a 同向向量）(3) 作用力＝反作用力
- **Force**：作用點、大小、方向 → 向量；單位 **N = kg·m/s²**
- **Torque（moment）= F × d**（d = 力作用線到旋轉軸的**垂直距離** = moment arm）；單位 **N·m**
- **Mechanical load** = force 或 moment
- 三種運動：**linear**、**angular**、**general**（兩者組合）
- **Mechanical equilibrium**：靜止或等速 → ΣF = 0、ΣM = 0
- **Free-body diagram**：只畫作用在該物體上的力，忽略環境與該物體施於他物的力
- 步態求解：**由遠端（足部、已知地面反作用力）往近端**；上一節段近端力 = 下一節段遠端力（大小相等方向相反）

## 2. 骨組織力學

### 2.1 成分與階層
- **Mineral 約 65%**（不純的 hydroxyapatite，含 carbonate、citrate、Mg、F、Sr）、**organic 約 35%**、細胞與水
- Organic matrix：**collagen 約 90%、NCP 約 10%**
- 五層階層：① collagen fibril ＋ carbonate apatite 晶體（數百 Å 長寬、**20–30 Å 厚**）→ ② mineralized collagen fibril → ③ 平行排列 → ④ 3D lamella → ⑤ **osteon**
- 每一層力學性質都不同

> **Pitfall（數字打架）**：OKU 15 Ch.13 用「有機 25–30%／無機 50–70%／水 5–10%、type I collagen 85–90%」；Ch.15 用「mineral 65%／organic 35%、collagen 90%」；OKU 14 Ch.14 用「HA 40%／collagen 35%／水 25%」。題目若給選項，選最接近「**礦物約 2/3、有機約 1/3、有機中 collagen 約 90%**」的答案。

### 2.2 骨的生物力學角色
- 保護器官：顱骨鈍傷能量集中於兩層骨板間的**海綿骨** → 內板與顱腔受保護
- 肌肉槓桿
- 長骨末端變寬 → **降低 stress（load/area）**，經關節下海綿骨傳到皮質骨
- 中耳：聲學放大與阻抗匹配

### 2.3 Whole-bone（structural）四參數 — 三點彎曲測試

| 參數 | 定義 | 意義 |
|---|---|---|
| **Stiffness** | load–displacement 曲線**線性區斜率** | 類似彈簧常數 K |
| **Maximum load（ultimate force）** | 測試中最大負荷 | 最簡單的強度指標 |
| **Ultimate displacement** | 從開始到斷裂的位移 | **ductility**；大 = ductile，小 = brittle（chalklike） |
| **Work-to-fracture** | **曲線下面積** | whole-bone **toughness** |

- **Yield point** 左側 = 彈性（卸載可回復）；右側 = **塑性（永久變形、損傷）**
- 三點彎曲測的是**中段骨幹（幾乎全皮質骨）**的 structural property
- **Stiffness 與 max load 高度相關**；**displacement 與兩者獨立**；work-to-fracture 受 displacement 與 max load 影響

**臨床對照**
- **Osteopetrosis**：很硬但很脆 → work-to-failure↓ → 骨折風險↑
- **幼童骨**：礦化差、弱，但**很 ductile** → work-to-failure↑ → **greenstick fracture**

**影響因子**
- **Morphology**：骨幹直徑大 → 更硬更強（但 displacement 主要由材料決定）
- **Material property**

### 2.4 Material（tissue-level, intrinsic）properties
- 以骨大小標準化（如 1×1×1 mm 立方體）；由 whole-bone 數據以 **beam theory** 推算
- Stress–strain 曲線彈性區斜率 = **Young modulus（E）** = 材料本質剛度
- 曲線下面積 = **toughness（modulus of toughness、energy absorption）**
- **Ultimate strength／ultimate strain**
- **關鍵觀念**：**intrinsic strength（MPa）與骨大小無關**；**ultimate load（N）隨骨大小而變** → 藥物或基因若改變骨大小，兩者趨勢可能不同

### 2.5 骨為何斷？
- 骨折風險與**吸收能量的能力**最相關，而非 strength 或 stiffness 本身
- **BMD 與 strength、stiffness 高度相關，但 Young modulus 與 ultimate strain 呈反比**
  - **鹿角**：礦化低、E 低、ultimate strain 高 → 極難折斷
  - **鯨魚 tympanic bulla**：礦化高、E 高、很脆（為聲學設計）
  - 長骨：介於中間；年輕牛骨比成熟牛骨較不硬也較不脆
- 高能量 → 粉碎；低能量 → 簡單骨折
- **骨最弱在 tension 與 shear，最強在 compression** → 裂縫沿張力或剪力面傳播

## 3. 肌腱與韌帶力學

- 韌帶：骨–骨，關節穩定；肌腱：肌–骨，傳遞肌力
- 高度水合；**type I collagen 佔乾重 75%–80%**
- **Elastin：韌帶 10%–15%、肌腱 <3%**（與 OKU 14 相同）
- 肌腱 collagen 沿受力方向均勻排列；韌帶較不規則
- **Proteoglycan** 對彈性貢獻小，但因分子巨大 → 主導**時間與負荷歷史依賴的 viscoelasticity**
- Type I collagen 組織都是**非線性彈性 → J-shaped／toe region**：低負荷時大變形 → 保護組織、enthesis 與骨骼免於損傷

## 4. 軟骨力學

**三種軟骨**

| 類型 | 特徵 | 部位 |
|---|---|---|
| **Hyaline**（最常見） | 光滑、藍白色 | **Articular cartilage** |
| **Elastic** | 黃色、富 elastin、**最柔韌** | 會厭、外耳、外耳道、耳咽管、喉 |
| **Fibrocartilage** | 粗大 collagen 纖維 | **Anulus fibrosus、半月板、部分 enthesis** |

**Articular cartilage**
- **Biphasic**（fluid：水；solid：collagen、proteoglycan、chondrocyte）＋ **viscoelastic**
- 組成與結構隨深度改變；剛度由 uncalcified → **tidemark** → calcified cartilage → subchondral bone 遞增 → **calcified zone 為過渡區，降低介面應力**
- Proteoglycan 變形受 collagen 限制 → 承受壓縮；solid matrix 對間隙水流動的摩擦 → **耗散能量**
- **Indentation test**：可見 **creep**；卸載時先**瞬間回復**，再**時間依賴回復**
- **Biphasic indentation creep 求三個 intrinsic properties**
  - **Aggregate modulus（H_A）**：由平衡位移、厚度、壓應力求得
  - **Poisson ratio（ν）**：決定 creep 曲線形狀
  - **Permeability（k）**：由 creep 速率（shift factor S = log₁₀(H_A·k/a²)，a = indenter 半徑）求得

## 5. 驗證與活體負荷

- 力學量測要有臨床用途必須**驗證與確認**
- 活體骨應變多以**直接貼在骨上的 strain gauge**＋遙測量測
- **OrthoLoad.com** = 最完整的活體關節負荷資料庫

## 6. 動作分析技術（新版重點）

- 傳統肉眼觀察（eyeballing）與理學檢查：**不準、再現性低、依賴主觀**

### 6.1 放射學方法
- **靜態 X 光**：起訖位置量 ROM；有輻射、非連續、難測節段旋轉、不可攜
- **Dynamic radiography（雙 fluoroscopy）**：3D 模型分析關節運動學；**輻射高、僅大型學術中心、最大 image intensifier 12 吋 → 動作範圍受限**、昂貴、需訓練

### 6.2 非放射學技術比較

| 技術 | 原理 | 優點 | 缺點 |
|---|---|---|---|
| **Optical（marker-based）** | 紅外線相機（**8–16 台**）＋反光標記，三角定位 | **Gold standard**、精準 | 昂貴、需受控空間（無反光面、固定光線）、需專人；**soft-tissue artifact 誤差至少 5°–10°** |
| **IMU** | accelerometer（線性加速度）＋ gyroscope（角速度）＋ magnetometer；sensor fusion | 輕巧、可在戶外／大空間 | **Drift**：誤差隨時間累積（magnetometer 協助校正）；soft-tissue artifact |
| **Markerless** | **深度相機（紅外線深度圖，低光可用）＋ RGB 相機＋ ML（CNN、RNN）** | 不需標記、自然、適用環境廣 | **精度低於 marker-based**；受光線、背景、遮擋影響；運算量大；**影像常需上傳外部伺服器 → 資安與隱私** |
| **Wearable** | 智慧手錶、fitness tracker；**smart shoe**（步態與足底壓力：plantar fasciitis、flatfoot） | 方便、即時回饋 | 消費級精度有限、配戴位置影響、隱私、成本 |
| **EMG** | 肌肉收縮電訊號 | 可結合 IMU 與 3D 模型 | 見下表 |
| **3D modeling（OpenSim）** | kinematics、kinetics、肌肉活化、moment arm；**inverse dynamics**（由動作求淨關節力矩）、**forward dynamics**（由肌肉活化預測動作） | 可個人化（CT／MRI 骨模型＋動作捕捉＋EMG） | 原始模型 **Gait2392** 來自**單一男性** → 已擴充至女性、兒童、特殊族群 |

**EMG 兩型**

| | Surface EMG | Intramuscular EMG |
|---|---|---|
| 方式 | 皮膚表面電極 | 細線或針電極插入肌肉 |
| 優點 | 非侵入、可同時監測多條肌肉 | 局部精確、可測深層肌 |
| 缺點 | 皮膚阻抗、電極位置、**相鄰肌 cross-talk** | 侵入、不適、需訓練 |

## 7. Finite Element Analysis（FEA）

- 將複雜結構切成 finite elements：2D（三角、四邊形）、3D（**tetrahedron、hexahedron**）
- 流程：幾何模型 → **mesh** → 材料性質＋邊界條件（約束、負荷）→ 迭代求解 → 應力分布、變形、失效點
- 優點：處理無法解析求解的複雜幾何與材料；原型製作前測試與優化
- **限制：準確度取決於 mesh 品質與輸入資料（材料性質、邊界條件）**；運算量大 → 不適合即時分析

---

## 8. 陷阱與易混淆

1. **Stiffness = 斜率；toughness／work-to-fracture = 曲線下面積**；max load = 曲線最高點
2. **Ultimate load（N）≠ intrinsic strength（MPa）**：前者受骨大小影響
3. **Osteopetrosis 硬而脆；兒童骨軟而 ductile（greenstick）**
4. **Young modulus 與 ultimate strain 反比**：礦化越高越硬也越脆
5. 骨**壓縮最強、張力與剪力最弱**
6. **Elastic cartilage 最柔韌**；**半月板與 anulus 是 fibrocartilage**
7. Cartilage biphasic 三參數：**H_A、ν、k**（不是 Young modulus）
8. IMU 的專屬誤差是 **drift**；optical 與 IMU 共有的誤差是 **soft-tissue artifact**
9. Markerless 的隱憂是**資料上傳外部伺服器的隱私**
10. 動作捕捉相機數：OKU 15 寫 **8–16 台**（OKU 14 寫 5–10 台）

---

## 9. Key Study Points（OKU 15）

- Mechanical load = 作用於肌肉骨骼系統的 force 或 moment
- Force 造成加速度或變形；torque 影響繞軸角運動
- 骨、肌腱、韌帶、軟骨的 stiffness、strength、ductility 決定其功能與對應力的反應
- 光學、IMU、markerless 系統與 AI／ML 整合提升動作捕捉精度與可用性
- **Soft-tissue artifact** 影響動作捕捉準確度，需進階技術降低

---

## 10. Anki 候選題

1. Load–displacement 曲線中，哪個參數代表 ductility？哪個代表 toughness？ → Ultimate displacement；work-to-fracture（曲線下面積）
2. 為何藥物研究中 ultimate load 與 ultimate strength 可能呈相反趨勢？ → Ultimate load 受骨大小影響（extrinsic），ultimate strength 是標準化後的材料本質（intrinsic）；藥物若改變骨大小，兩者可不同向
3. 骨最容易在哪兩種負荷下失效？ → Tension 與 shear
4. Biphasic indentation creep 可求得 articular cartilage 哪三個本質參數？ → Aggregate modulus（H_A）、Poisson ratio（ν）、permeability（k）
5. IMU 特有的誤差來源是什麼？如何減輕？ → Drift（gyroscope／accelerometer 誤差累積）；magnetometer 協助維持方位準確
6. OpenSim 的 inverse dynamics 與 forward dynamics 差在哪？ → Inverse：由觀察到的動作計算淨關節力矩與力；forward：由指定的肌肉活化與外力預測動作

---

*本頁為 OKU 15 原文（OCR）與 OKU 14 筆記逐段比對後，以中文自行整理的差異重點，非原文翻譯；數值以原書為準。*
