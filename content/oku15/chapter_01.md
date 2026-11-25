---
title: "OKU 15 Ch.1: Orthopaedic Research（OKU 14 CH1 更新）"
date: 2026-11-25
draft: false
tags: ["OKU15", "General Topics", "Research Methods", "版本差異"]
categories: ["OKU 15 更新"]
weight: 1
summary: "篇幅 8 → 10 頁，由 Ch.2 的同一位作者重寫。研究設計從 OKU 14 的 CH2 移到這一章；新增 PICOT 與 FINER、bias 類型表、GRADE 的升級與降級規則、IOM 可信賴 CPG 標準、registry-based RCT 等新研究方法。Fixed vs random effects 和 Cochrane RoB 的細節不再涵蓋。"
---

> **對照：**OKU 14 [CH1 Orthopaedic Research]({{< relref "/chapter_01.md" >}}) → OKU 15 **Ch.1**（同名）｜PDF 8 → 10 頁｜作者是 OKU 15 Ch.2 的同一人
>
> **來源說明：**OKU 15 這章是掃描檔，本頁根據 OCR 文字整理。
>
> **閱讀方式：**🆕 新增；🔄 改變；✅ 一致；❌ OKU 15 不再涵蓋。

## 0. 考點變更總表

| 主題 | OKU 14 CH1 | OKU 15 Ch.1 | 類型 |
|---|---|---|---|
| 研究類型 | Translational science spectrum | Basic science、clinical、translational 三類，translational 分 **5 個階段**（NCATS spectrum） | ✅ |
| 研究問題的建構 | **PICO** | **PICOT**（多了 Time）＋ 🆕 **FINER** | 🔄 |
| 研究設計分類 | 在 OKU 14 的 **CH2** | 移到這一章：observational vs experimental 對照表 | 🔄 |
| Bias | Cochrane RoB 的各項參數 | 🆕 **常見 bias 類型表**（selection、attrition、response、information、recall、confounding、publication） | 🔄 |
| Meta-analysis 模型 | Fixed vs random effects 比較表 | **不再涵蓋** | ❌ |
| 報告規範 | PRISMA 2020、MOOSE、AMSTAR 2 | PRISMA、MOOSE ✅；另提到評估 SR 品質的工具 | ✅ |
| Levels of evidence | JBJS 分級 | 同樣的 JBJS 表（therapeutic、prognostic、diagnostic、economic）＋ 🆕 **Oxford CEBM 2011** 依臨床問題分級 | 🔄 |
| GRADE | 流程概述 | 🆕 **證據品質的升級與降級規則**（見 3.2） | 🆕 |
| 建議強度 | Strong、moderate、limited、consensus | 相同；AAOS 另外考量效益與風險的取捨、效果大小、關鍵結果 | ✅ |
| CPG 標準 | National Academy of Medicine 定義、AAOS 流程 | 🆕 **IOM 可信賴 CPG 的八項標準** | 🆕 |
| 未來研究方法 | — | 🆕 **Registry-based RCT、network meta-analysis、real-world data（EMR）、ML／NLP**、population registry | 🆕 |

---

## 1. 研究的類型 ✅
- **Basic science**（bench research）：實驗室、動物、生理實驗，探討機轉，開發新材料與療法。
- **Clinical research**：以人為對象，評估藥物、器材、治療的效果與安全性，前提是要有 in vitro 與 in vivo 的臨床前資料。
- **Translational research**：從 bench 到 bedside 再到 practice（社區與公衛）。共 **5 個階段**（NCATS translational science spectrum），階段之間不一定依序進行，後期的結果可能回饋到前期。

## 2. 執行研究的四步驟
1. **提出研究問題**
2. **搜尋最佳證據**
3. **批判性評估證據**
4. **下結論，並推廣到臨床實務**

### 2.1 PICOT 🔄
| 字母 | 內容 |
|---|---|
| **P**opulation | 研究對象、招募方式、納入與排除條件 |
| **I**ntervention | 介入細節、副作用，以及與標準治療相比是否恰當 |
| **C**omparison | 對照組；**使用安慰劑或不給 gold standard 的倫理問題** |
| **O**utcome | 以經過驗證、可靠的工具量測，會影響統計計畫與 power |
| **T**ime 🆕 | 研究期間、追蹤時間、資料收集頻率，以及**如何避免失訪** |

### 2.2 FINER 🆕
| 字母 | 意義 |
|---|---|
| **F**easible | 病人數、團隊專業、資源足夠，結果可以量測 |
| **I**nteresting | 研究者、讀者、經費來源都感興趣 |
| **N**ovel | 能產生新假說，或延伸過去的發現 |
| **E**thical | 保護病人隱私與安全 |
| **R**elevant | 對科學、臨床或政策有貢獻，能帶動後續研究 |

> 兩個模型都強調 **feasibility**：病人數是否足以用恰當的統計回答問題、資源是否足以完成全部階段。

## 3. 評估證據

### 3.1 研究設計 🔄（自 OKU 14 CH2 移來）
| 類別 | 設計 | 重點 |
|---|---|---|
| Observational | **Cohort** | 追蹤一群人的暴露與結果，可以是 retrospective 或 prospective |
| | Cross-sectional | 單一時間點 |
| | **Case-control** | 依「有沒有結果」分組，比較暴露 |
| | Case series | 少數有特定結果或暴露的病人 |
| Experimental | **Randomized blinded trial** | 隨機分組，病人不知道接受哪種處置 |
| | Controlled clinical trial | 有對照組但沒有隨機分派 |
| | Uncontrolled trial | 沒有對照組 |
| Filtered | **Systematic review、meta-analysis** | 綜合多個研究 |

- **RCT 是 gold standard，但不一定可行或合乎倫理**，耗費資源大，結果也不一定能推廣到一般病人。
- SR 和 meta-analysis 可以彌補單一研究推廣性的不足，但**必須評估納入研究的品質與 bias**。RCT 的 SR 依 **PRISMA**，觀察性研究的 SR 依 **MOOSE**。

### 3.2 Bias 🆕（觀念題）
| Bias | 定義 |
|---|---|
| **Selection** | 選入研究的人與未選入的人有系統性差異 |
| **Attrition** | Selection bias 的一種：病人退出或失訪 |
| **Response** | 有回應者與沒回應者有系統性差異 |
| **Information／measurement** | 暴露或結果被錯誤報告或分類，或使用未經驗證的工具 |
| **Recall** | 病人回憶的能力不同，或記憶有誤 |
| **Confounding** | 外在變數影響了結果，應該在分析時控制 |
| **Publication** | 陽性或顯著的結果比較容易被發表 |

- 降低 bias 的方法：恰當的隨機分派、嚴謹的資料收集與管理、確保追蹤完整、使用適當的統計方法。

### 3.3 證據等級 🔄
- 證據金字塔依 **bias 的多寡**排序：**filtered（SR、MA）> RCT > 控制較少的研究 > case series 與 expert opinion**。
- JBJS 的 levels of evidence 分成四類研究問題：**therapeutic、prognostic、diagnostic、economic／decision analysis**，各有 Level I–V。
  - 例：**Therapeutic Level I 是 RCT**（有顯著差異，或無差異但 CI 夠窄）；**follow-up < 80% 的 RCT 降為 Level II**。
  - **Prognostic Level I 是 prospective inception cohort，且追蹤 > 80%**。
  - **Diagnostic Level I** 是在連續病人中驗證已建立的診斷標準，並普遍使用 gold standard。
- 🆕 **Oxford CEBM（2011）**依臨床問題分級：盛行率、診斷或監測準確度、預後、治療的效益與傷害、篩檢。

### 3.4 GRADE 🆕
- **證據品質分四級：high、moderate、low、very low**，代表研究者有多大把握「真正的效果接近估計值」。
- **起始等級：RCT 從 high 開始，observational study 從 low 開始。**
- **降級因素（各 −1 或 −2）：**risk of bias、inconsistency、indirectness、imprecision、publication bias。
- **升級因素（主要用於 observational study）：**
  - 效果很大（+1 或 +2）
  - 有 dose-response（+1）
  - 所有合理的干擾因子都會「削弱」所見的效果（+1）

> **記法：**降級五項是「**偏、不一致、不直接、不精確、發表**」；升級三項是「**效果大、劑量反應、干擾因子反向**」。

### 3.5 建議強度 ✅
- **Strong、moderate、limited、consensus**，與 OKU 14 相同。
- AAOS 另外納入：證據品質與數量、**效益與傷害的取捨**、效果大小、是否有關鍵結果的資料，以及資源、公平性、病人價值與偏好。也會評估未來研究推翻現行建議的可能性。

## 4. 推廣到臨床：CPG 🆕
- **IOM 自 1990 年起**定義 CPG，並訂出可信賴 CPG 的標準：
  1. **透明**：流程公開
  2. **利益衝突管理**：揭露與撤資是強制的
  3. **團隊組成**：跨領域、平衡，包含臨床醫師與方法學專家
  4. **與 SR 的結合**：依 SR 的標準記錄搜尋、納入與排除
  5. **證據基礎與建議強度**：每項建議都說明理由、強度與證據品質
  6. **明確表述建議**：標準化的建議行動與監測
  7. **外部審查**：涵蓋所有利害關係人
  8. **定期更新**：有新證據時就修訂
- AAOS 網站的 CPG 會定期更新（依 AAOS CPG methodology v4.0，2023）。

## 5. 未來的研究方向 🆕
- 骨科常見的困境：比較手術術式時，RCT 不見得合乎倫理或可行。
- 替代方法：
  - **Registry-based RCT**
  - **Network meta-analysis**
  - **Real-world data**（以 EMR 為基礎的研究）
  - **Machine learning、NLP**
  - **Population-based registry**：可以看大量病人的長期結果，適合爭議多年的手術技術問題

---

## 6. OKU 14 CH1 中 OKU 15 不再涵蓋的內容 ❌
- **Fixed-effect vs random-effects model** 的比較
- Cochrane risk of bias tool 的各項參數（allocation concealment、blinding 等）
- AMSTAR 2 的細節
- 內部與外部效度的提問矩陣

---

## 7. Anki 候選題

1. PICOT 的 T 代表什麼？→ Time：研究期間、追蹤時間、資料收集頻率，以及如何避免失訪。
2. FINER 的五個字母分別代表什麼？→ Feasible、Interesting、Novel、Ethical、Relevant。
3. Attrition bias 屬於哪一類 bias？→ Selection bias（病人退出或失訪）。
4. GRADE 中，RCT 和 observational study 的起始證據等級？→ RCT 從 high 開始，observational study 從 low 開始。
5. GRADE 的五個降級因素？→ Risk of bias、inconsistency、indirectness、imprecision、publication bias。
6. GRADE 的三個升級因素？→ 效果很大、dose-response、所有干擾因子都會削弱所見效果。
7. Follow-up < 80% 的 RCT 屬於哪一級？→ Therapeutic Level II。
8. Prognostic Level I 的條件？→ Prospective inception cohort，追蹤 > 80%。
9. AAOS 的四種建議強度？→ Strong、moderate、limited、consensus。
10. RCT 的 SR 和觀察性研究的 SR 各依循什麼報告規範？→ PRISMA；MOOSE。
11. 不適合做 RCT 時，可以用哪些替代研究方法？→ Registry-based RCT、network meta-analysis、real-world data（EMR）、population registry、ML／NLP。

---

*本頁為 OKU 15 原文（OCR）與 OKU 14 筆記逐段比對後，以中文自行整理的差異重點，非原文翻譯；數值以原書為準。*
