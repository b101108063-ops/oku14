---
title: "OKU 15 Ch.8: Musculoskeletal Imaging Principles（OKU 14 CH9 更新）"
date: 2026-11-25
draft: false
tags: ["OKU15", "General Topics", "Imaging", "版本差異"]
categories: ["OKU 15 更新"]
weight: 8
summary: "篇幅 14 → 16 頁，作者重寫，從「基本原理與檢查選擇」改成「近年新技術總覽」。新增 UHF MRI（7T 於 2017 年經 FDA 核准）、UTE、MR neurography、MR elastography、whole-body MRI（myeloma）、DWI／DTI、chemical shift、DCE-MRI、dual-energy CT、weight-bearing CT、cone beam CT、photon-counting CT、PET-MRI、超音波新技術、radiomics 與 synthetic imaging。OKU 14 的各檢查適應症、輻射安全、MRI 序列判讀、MARS、臨床影像流程都不再涵蓋。"
---

> **對照：**OKU 14 [CH9 Musculoskeletal Imaging Principles]({{< relref "/chapter_09.md" >}}) → OKU 15 **Ch.8**（同名）｜PDF 14 → 16 頁｜作者群全新
>
> **來源說明：**掃描檔，本頁根據 OCR 文字整理。
>
> **閱讀方式：**🆕 新增；🔄 改變；✅ 一致；❌ OKU 15 不再涵蓋。
>
> 💡 **讀法建議：**OKU 15 這章是**新技術清單**，每項的考法多半是「哪一種技術最適合看什麼」。**基本原理**（X 光、CT、MRI 序列、核醫的選擇、輻射安全）**仍以 OKU 14 CH9 為主**。

## 0. 考點變更總表

| 主題 | OKU 14 CH9 | OKU 15 Ch.8 | 類型 |
|---|---|---|---|
| 章節定位 | 各檢查的原理、適應症與臨床影像流程 | **近年新技術的總覽**：原理、應用、限制 | 🔄 |
| X 光、透視、DXA、核醫、輻射安全 | 有 | **不再涵蓋** | ❌ |
| MRI 物理與四種常用序列、金屬假影抑制（MARS）、顯影劑原則、磁場強度 | 有 | 只保留**磁場強度**（3T → UHF），其餘不再涵蓋 | ❌／🔄 |
| 臨床影像流程（創傷、關節炎、腫瘤、感染、術前規劃） | 有 | **不再涵蓋** | ❌ |
| 進階 MRI | — | 🆕 UHF、軟骨影像、inversion、**UTE**、3D MRI、**neurography**、**MR elastography**、**whole-body MRI**、兒童 MRI、**T1ρ**、MRI 生物力學、**DWI**、**DTI**、**chemical shift**、**DCE** | 🆕 |
| 進階 CT | — | 🆕 **Dual-energy CT**、**weight-bearing CT**、CT 導引 3D 列印、**cone beam CT**、**photon-counting CT**、**PET-MRI** | 🆕 |
| 超音波 | 簡介 | 🆕 POCUS、quantitative US、**elastography**、**superb microvascular imaging**、CEUS、image fusion | 🆕 |
| AI | — | 🆕 自動判讀、**radiomics**、個人化影像、**synthetic MRI／CT** | 🆕 |

---

## 1. MRI 新技術 🆕

### 1.1 磁場強度
- **3T（2000 年代初期）**相比 1.5T：掃描效率更高、影像品質更好、看得到更細的結構，並能支援 quantitative MRI、neurography、不打顯影劑的軟骨影像。
- **UHF（ultra-high field）：5T、7T、9.4T。**SNR 與 CNR 更高，解析度更好、掃描時間更短。**7T 在 2017 年經 FDA 核准臨床使用。**
  - 骨科應用：**不打顯影劑的高解析關節軟骨影像與 mapping**（膝、髖、踝），早期軟骨或半月板病變，骨骼肌，以及骨折和骨鬆的**骨小樑微結構**。
  - 缺點：昂貴、不普及、法規限制、**磁場不均勻造成的假影**。
- 磁場強度提升也讓影像從 **arthrogram 逐漸轉向不打顯影劑的影像**。

### 1.2 新序列與技術速查

| 技術 | 原理 | 骨科應用 | 限制 |
|---|---|---|---|
| **軟骨影像** | 傳統用 T2、**PDFS**；進階：**dGEMRIC**（要打 gadolinium）、**T2 mapping**、彩色 mapping（不需顯影劑） | 退化性關節病、外傷性軟骨損傷 | — |
| **Inversion imaging** | 後處理，把灰階反轉以增加對比 | **Bony Bankart、pars defect**、FAI、肩關節唇與 rotator cuff、**hardware 失敗與鬆脫** | 判讀者不熟悉可能誤讀 |
| **UTE（ultrashort echo time）** | TE 縮短到微秒等級（比一般短 100–1,000 倍），**在訊號衰減前擷取短 T2 組織的訊號** | **肌腱、韌帶、半月板**（傳統 MRI 上是黑的）、**金屬植入物**（減少假影，看鬆脫或感染）、**皮質骨** | 硬體與軟體昂貴，**對移動非常敏感** |
| **3D MRI** | 直接擷取 isotropic 立體資料 | **小關節**（腕 TFCC、踝肌腱）、斜走的結構（周邊神經） | 掃描時間長、成本高 |
| **MR neurography** | 脂肪抑制、顯影與高解析 3D 序列 | **神經損傷、壓迫（如 CTS）、神經腫瘤**；**failed back surgery 中非椎間盤的疼痛來源** | — |
| **MR elastography** | 外加振動產生剪力波，繪製**組織硬度圖** | **不必切片就能評估神經與肌肉疾病**（纖維化、神經損傷） | 設備複雜、振動造成不適 |
| **Whole-body MRI** | 一次掃描全身 | **Multiple myeloma**（診斷、分期、追蹤）、骨轉移、發炎性關節炎、**CRMO**、肌炎、SLE、系統性硬化症 | 不普及、耗時、移動假影、昂貴 |
| **兒童 MRI** | 快速序列（compressed sensing、radial），減少鎮靜與移動假影；**ferumoxytol** 顯影劑（可生物分解，**沒有 NSF 風險**） | — | — |
| **T1ρ（quantitative MRI）** | 旋轉座標系中的縱向弛豫，對大分子環境的變化敏感 | 軟骨退化、半月板、骨髓水腫、脊椎退化 | 對移動敏感、不普及、耗時 |
| **MRI 生物力學** | Bone statistical shape modeling；關節運動學；**4D 動態 MRI** | 預測膝 OA 進展（潛在的 biomarker）、ACLR 後的運動學 | 掃描機內空間有限 |
| **DWI** | 量測水分子的擴散 | **腫瘤與治療反應**、**區分病理性骨折的類型**、退化、區分發炎、感染與惡性 | 移動、空氣與組織交界的假影；**T2 shine-through**（血管性腫瘤在 T2 上可能像液體） |
| **DTI** | 多方向擴散的 tensor 模型 | 脊椎韌帶、椎間盤、**脊髓與神經根完整性**（spinal stenosis）、軟組織發炎與腫瘤 | — |
| **Chemical shift（Dixon）** | 利用脂肪與水質子的共振頻率差異 | **區分良性與惡性骨髓病灶**；肌腱、肌肉、椎間盤、脊椎腫瘤與感染 | 只能分辨水和脂肪 |
| **DCE-MRI** | 顯影後連續掃描，得到 time-intensity curve | **區分良性與惡性病灶**、軟骨病變、術後變化 | 顯影劑過敏、需要靜脈注射 |

### 1.3 Whole-body MRI 與 myeloma 🆕（指引題）
- **NICE：疑似 myeloma 時建議做 whole-body MRI**；追蹤復發或惡化時，再合併 spine MRI 與 **FDG PET-CT**。
- **Oxford CEBM：**支持用 whole-body MRI 為各類 myeloma 分期。
- **British Society for Haematology：**支持用 whole-body MRI 追蹤治療反應。
- **MY-RADS（2019）**：統一 whole-body MRI 的掃描、判讀與報告方式。
- 有無法取出的金屬植入物時，可以改用 **1.5T**。

### 1.4 Chemical shift 判讀
- 原書附圖的例子：**out-of-phase 影像訊號下降超過 20%**，符合**良性的 focal marrow hyperplasia**。訊號沒有下降，表示病灶內沒有脂肪，要懷疑惡性。

## 2. CT 新技術 🆕
- 近年 CT 的發展方向是**看軟組織（不只是骨頭）**，以及**降低輻射劑量**。

| 技術 | 原理 | 應用 | 限制 |
|---|---|---|---|
| **Dual-energy CT** | 兩種能量的 X 光（例如 rapid kVp switching），可以區分 **calcium、iodine、軟組織** | **BMD 測量**（腰椎的 3D 評估比 DXA 更準）、骨與軟組織病灶、**痛風（尿酸結晶）**、**骨髓水腫** | 輻射劑量增加、需要特殊設備 |
| **Weight-bearing CT** | **站立承重下**的 3D 影像 | OA、關節不穩定、脊椎排列、術前規劃 | 劇痛或不穩定的病人難以配合 |
| **CT 導引 3D 列印** | 利用 CT 的高解析骨骼影像建模 | 骨模型、**手術導板**、特殊植入物、scaffold、骨移植；已有醫院在放射科內設立 3D 列印 | 成本效益 |
| **Cone beam CT** | **錐狀 X 光束加 flat-panel detector**，視野窄 | **weight-bearing CT 與肢體影像**；**輻射比傳統 CT 低** | 軟組織對比差、昂貴 |
| **Photon-counting CT** | **逐一計數 X 光光子** | **細微骨折**、**減少金屬假影**（beam hardening 較少）；對比與解析度更好，**劑量更低** | 昂貴、需要特殊設備與訓練 |
| **PET-MRI** | PET 功能影像加 MRI 解剖影像 | **肌肉骨骼腫瘤**、**慢性骨髓炎**、發炎性關節病；**軟組織對比最好、沒有游離輻射** | 不普及、昂貴 |

> 原書圖例：PET-MRI 在 subscapularis 與 glenoid 之間找到一個小病灶，切片證實是 **phosphaturic mesenchymal tumor**（造成 tumor-induced osteomalacia 的腫瘤）。

## 3. 超音波新技術 🆕

| 技術 | 原理與應用 | 限制 |
|---|---|---|
| **POCUS（point-of-care US）** | 急診、加護病房、運動場邊的即時評估，**已擴展到上肢與兒童骨折的診斷** | — |
| **Quantitative US** | 量化組織密度與彈性 | 用於骨鬆、肌腱與肌肉傷害、骨與肌肉量疾病 |
| **US elastography** | 施加壓力或振動，觀察組織變形，繪製硬度圖；用於**腫瘤**、肌腱病、肌肉拉傷、韌帶損傷 | 依賴操作者，深部結構難評估 |
| **SMI（superb microvascular imaging）** | 高解析的**微血管血流影像**；用於肌腱損傷、**腱鞘炎**（如 de Quervain）、肌肉撕裂、血管疾病、**肢體延長時的兒童新骨生成** | 依賴操作者，深部血管看不到 |
| **CEUS** | 微氣泡顯影劑，評估血流與灌流；用於軟組織腫瘤、肌腱與肌肉傷害 | 需要特定顯影劑與設備 |
| **Image fusion US** | 即時超音波疊合 CT、MRI 或 PET，**導引注射或切片** | 需要精確對位與先進軟硬體 |

## 4. AI 與影像 🆕
- **自動判讀：**骨齡、骨病灶、植入物位置、關節置換的併發症。
- 挑戰：各家掃描流程不一致、**overfitting**、可解釋性不足、難以整合到臨床流程。
- **Radiomics：**用演算法從影像擷取**紋理、形狀、強度等量化特徵**，提供肉眼看不到的資訊。
  - 應用：**腫瘤特性**（良惡性、分級與亞型、治療反應）、**骨質與骨折風險**、**個人化影像**（依病人調整參數、輻射劑量與顯影劑）。
- **Synthetic imaging：**
  - **Synthetic MRI**：**一次掃描產生 T1、T2、PD 等多種對比**，縮短掃描時間。
  - **Synthetic CT**：**從 MRI 或 PET 資料產生類似 CT 的骨骼影像，不需要額外輻射**，適合兒童或需要反覆追蹤的病人。品質受原始影像限制，無法完全取代 CT。

---

## 5. OKU 14 CH9 中 OKU 15 不再涵蓋的內容 ❌（基本原理，請保留 OKU 14 筆記）
- X 光、透視、DXA、CT、MRI、超音波、核醫各自的原理與適應症
- **輻射安全**（劑量、ALARA、孕婦、兒童）
- **MRI 物理**（T1、T2 弛豫）與**四種常用序列的訊號判讀**
- **金屬假影抑制（MARS）**
- **顯影劑使用原則**（含 NSF）
- 創傷、關節炎、腫瘤、感染的**臨床影像流程**，以及核醫檢查的選擇
- 影像假影與常見誤讀陷阱

---

## 6. Anki 候選題

1. 7T MRI 何時經 FDA 核准臨床使用？→ 2017 年。
2. UHF MRI 在骨科的主要優點？→ 不打顯影劑的高解析軟骨影像與 mapping、骨小樑微結構。
3. 傳統 MRI 上肌腱為什麼是黑的？哪一種技術可以看到？→ T2 弛豫時間很短；UTE MRI。
4. Inversion imaging 適合找哪些病灶？→ Bony Bankart、pars defect、hardware 失敗或鬆脫。
5. 評估周邊神經壓迫或神經腫瘤，用哪一種 MRI 技術？→ MR neurography。
6. 不必切片就能評估肌肉或神經硬度的 MRI 技術？→ MR elastography。
7. NICE 建議疑似 multiple myeloma 時做什麼影像？→ Whole-body MRI。
8. 兒童 MRI 的新顯影劑及其優點？→ Ferumoxytol，可生物分解、沒有 NSF 風險。
9. 區分良性與惡性骨髓病灶的 MRI 技術？判讀原則？→ Chemical shift（Dixon）；out-of-phase 訊號下降超過 20% 偏向良性。
10. DWI 判讀時的 T2 shine-through 陷阱是什麼？→ 血管性腫瘤在 T2 上可能看起來像液體。
11. 能看出尿酸結晶（痛風）的 CT 技術？→ Dual-energy CT。
12. Dual-energy CT 在骨密度測量上的優勢？→ 腰椎 3D 評估比 DXA 更準。
13. Cone beam CT 與傳統 CT 的差異？→ 錐狀光束加 flat-panel detector，視野窄、輻射較低，但軟組織對比差。
14. 能減少金屬假影、偵測細微骨折的新型 CT？→ Photon-counting CT。
15. 哪一種混合影像的軟組織對比最好、又沒有游離輻射？→ PET-MRI。
16. 看腱鞘炎微血管血流的超音波技術？→ Superb microvascular imaging（SMI）。
17. Radiomics 是什麼？→ 用演算法從影像擷取量化特徵（紋理、形狀、強度）。
18. 不需要額外輻射就能得到類似 CT 骨骼影像的技術？→ Synthetic CT（由 MRI 或 PET 資料產生）。

---

*本頁為 OKU 15 原文（OCR）與 OKU 14 筆記逐段比對後，以中文自行整理的差異重點，非原文翻譯；數值以原書為準。*
