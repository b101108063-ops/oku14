---
title: "OKU 15 Ch.2: Biostatistics（OKU 14 CH2 更新）"
date: 2026-11-25
draft: false
tags: ["OKU15", "General Topics", "Biostatistics", "版本差異"]
categories: ["OKU 15 更新"]
weight: 2
summary: "篇幅 12 → 6 頁，作者重寫。研究設計、PROM 術語、fragility index 都不再涵蓋；改以假設檢定流程、ASA 六項 P 值原則、effect size 指標的大小界值、MCID、CI、Bonferroni 與統計檢定選擇表為主。注意：原書 type I／II error 的文字定義寫反了。"
---

> **對照：**OKU 14 [CH2 Biostatistics]({{< relref "/chapter_02.md" >}}) → OKU 15 **Ch.2**（同名）｜PDF 12 → 6 頁（−50%）｜單一作者，全章重寫
>
> **閱讀方式：**🆕 新增；🔄 改變；✅ 一致；❌ OKU 15 不再涵蓋；⚠️ 原書疑似錯誤。

## 0. 考點變更總表

| 主題 | OKU 14 CH2 | OKU 15 Ch.2 | 類型 |
|---|---|---|---|
| 研究設計（descriptive vs analytic、RCT／cohort／case-control） | 主要內容之一 | **不再涵蓋**（可能移到 Ch.1 Orthopaedic Research） | ❌ |
| PRO／PROM／PRO-PM、MIC、MID、MDC、PASS | 詳細的術語表 | 只保留 **MCID**，並以 ASES 為例 | ❌／🔄 |
| Fragility index、fragility quotient | 有 | **不再涵蓋**（只出現在參考文獻） | ❌ |
| 假設檢定流程 | 原則 | 明列步驟：選檢定 → 設 H0／H1 → 計算 power 與樣本數 → 算 P 值、CI、effect size → 依 MCID 判斷臨床意義 | 🔄 |
| **ASA 對 P 值的六項原則** | 未列 | 🆕 逐條列出 | 🆕 |
| Effect size 指標與大小界值 | 未列 | 🆕 Cohen d、OR、RR、Pearson r、r² 的小／中／大界值 | 🆕 |
| 樣本數 | 計算要素 | 加上 effect size × power 的樣本數對照表 | 🔄 |
| 統計檢定選擇 | 多元資料與資料型態 | 🆕 **完整的檢定選擇表**（parametric、nonparametric、categorical） | 🆕 |
| Normality | — | **n ≥ 30 可假設常態**（central limit theorem）；常態檢定 Shapiro-Wilk 等 | 🆕 |
| Type I／II error 的定義 | 正確 | ⚠️ **原書正文把兩者的文字定義寫反了**（見 1.1） | ⚠️ |

---

## 1. 假設檢定

### 1.1 Type I／II error ⚠️（一定要記對）
- **H0（null）**：變數之間沒有關聯。**H1（alternative）**：有關聯。
- **正確的定義：**
  - **Type I（α）error = false positive**：實際上沒有差異，研究卻判定有差異，錯誤地拒絕了 H0。
  - **Type II（β）error = false negative**：實際上有差異，研究卻沒有偵測到，錯誤地未拒絕 H0。
- ⚠️ **OKU 15 正文的文字定義寫反了**：它把「實際上有關係卻判定沒有」稱為 type I，把「實際上沒差卻判定有差」稱為 type II。但同一章的 Figure 1 二乘二表標示是正確的，與標準定義一致。**考試請以標準定義作答。**
- **α 通常設 0.05。**多重檢定或漏掉重要發現的代價較高時，可以把 α 設得更嚴格（如 0.01）。
- **β 通常設 0.10 或 0.20**，也就是 **power 90% 或 80%**。**Power = 1 − β**，即避免 type II error 的機率。

### 1.2 Power 與樣本數 🔄
- **研究開始前一定要做 power analysis。**需要的資訊：使用的檢定、α、母群體的變異數，以及想偵測的 effect size。
- **提高 power 的方法：**擴大要偵測的 effect size、增加樣本數、放寬 α、降低測量誤差。
- 🆕 **樣本數與 effect size 的關係**：effect size 愈小，需要的樣本數增加得愈快。以標準化 effect size 0.5、power 80% 為例，每組約需 60 多人；effect size 降到 0.1 時，每組需要超過 1,500 人。考試考的是這個趨勢，不考精確數字。

### 1.3 P 值 🆕
- **定義：**假設 H0 為真時，得到等於或比觀察結果更極端之結果的機率。
- **0.05 這個門檻其實很武斷**，原本並不是要當作硬性的決策點。
- **ASA（American Statistical Association）的六項原則**（重點改寫）：
  1. P 值反映資料與特定統計模型**不相容的程度**。
  2. P 值**不是**「假設為真的機率」，也**不是**「結果純屬機率造成的機率」。
  3. 科學結論與決策**不應只看 P 值是否過門檻**。
  4. 正確的推論需要**完整報告與透明**。
  5. P 值和統計顯著性**不代表效果大小或重要性**。
  6. 單獨一個 P 值**不是好的證據指標**。

> **考點：**選項中只要出現「P = 0.03 代表 H0 為真的機率是 3%」或「P 值愈小效果愈大」，就是錯的。

## 2. 臨床意義

### 2.1 Effect size 🆕

| 指標 | 用途 | 小／中／大 |
|---|---|---|
| **Cohen d** | 兩組平均數差 ÷ SD | **0.2／0.5／0.8** |
| Odds ratio | 兩組 odds 的比值（= 1 代表相同） | 1.5／2.0／3.0 |
| Relative risk | 兩組機率的比值（= 1 代表相同） | 2.0／3.0／4.0 |
| Pearson r | 線性相關，範圍 −1 到 +1 | ±0.2／±0.5／±0.8 |
| r²（coefficient of determination） | 一個變數可解釋的變異比例，0 到 1 | 0.04／0.25／0.64 |

- **Absolute effect size**：兩組結果的差（或標準化差）。**Relative effect size**：比較兩組關聯強度。

### 2.2 MCID 🔄
- 定義：**病人或醫師能察覺、對病人有益的最小變化。**
- 大型研究可能統計顯著，但沒有臨床意義。
- 例子：**ASES 的 MCID 依診斷與治療不同，從約 6.4 分到超過 17 分（滿分 100）**，所以要依病人情境解讀。
- OKU 14 的 MIC、MID、MDC、PASS、anchor-based 與 distribution-based 等內容，新版不再展開。

### 2.3 Confidence interval ✅
- 影響 CI 寬度的因素：**樣本數、樣本變異、信心水準**（通常 95% 或 99%）。

### 2.4 Multiple comparisons ✅
- 做愈多次檢定，type I error 的總機率愈高。
- **Bonferroni 校正：每個檢定的 α = 整體 α ÷ 檢定數**。例如 10 個檢定時，每個用 0.005。
- 代價是 power 下降，type II error 增加。

## 3. 選擇統計檢定 🆕

### 3.1 選擇前要問的問題
自變項幾個？各是什麼資料型態？依變項是什麼型態？觀察值是獨立還是配對？比的是平均數、中位數，還是相關性？

### 3.2 資料型態
- **Numeric**：discrete（計數）、continuous。
- **Categorical**：ordinal（有順序）、nominal（無順序，如種族、保險別）、binary。
- **Parametric**（常態分布）vs **nonparametric**（非常態、分布未知或樣本很小）。**n ≥ 30 一般可假設常態**，依據是 central limit theorem。

### 3.3 常用檢定速查

| 研究問題 | Parametric | Nonparametric | Categorical |
|---|---|---|---|
| 兩組，不配對 | Unpaired t-test | **Mann-Whitney U**（= Wilcoxon rank-sum） | **Chi-square**；小樣本用 **Fisher exact** |
| 三組以上，不配對 | **ANOVA** | **Kruskal-Wallis** | Chi-square |
| 兩組，配對 | Paired t-test | **Wilcoxon signed-rank** | **McNemar** |
| 三組以上，配對 | Repeated-measures ANOVA | **Friedman** | **Cochran Q** |
| 相關 | **Pearson** | **Spearman**、Kendall | RR、OR |
| 一致性 | **Bland-Altman**、ICC | — | **Cohen kappa** |
| 預測 | Linear regression | — | **Logistic regression**（二元結果） |
| 存活分析 | **Kaplan-Meier**、**log-rank**、**Cox proportional hazards** | | |
| 常態性檢定 | **Shapiro-Wilk**、Anderson-Darling、Kolmogorov-Smirnov | | |

---

## 4. Anki 候選題

1. Type I error 是什麼？→ False positive：實際上沒有差異卻判定有差異（錯誤拒絕 H0）。注意原書正文寫反了。
2. Power 的定義？→ 1 − β，即真的有差異時能偵測到的機率。
3. 提高 power 的四種方法？→ 增加樣本數、擴大 effect size、放寬 α、降低測量誤差。
4. P 值能告訴你假設為真的機率嗎？→ 不能（ASA 原則）。
5. Cohen d 的小／中／大界值？→ 0.2／0.5／0.8。
6. r² = 0.25 代表什麼？→ 中等關聯，可以解釋 25% 的變異。
7. 做 10 個檢定，整體 α = 0.05，Bonferroni 校正後每個檢定的 α？→ 0.005。
8. 兩組不配對、非常態的連續資料，該用什麼檢定？→ Mann-Whitney U（Wilcoxon rank-sum）。
9. 配對的類別資料（例如治療前後是否疼痛），該用什麼檢定？→ McNemar test。
10. 評估兩位觀察者對類別判讀的一致性，該用什麼？→ Cohen kappa；連續資料用 ICC 或 Bland-Altman。
11. 樣本數多少可以假設常態？依據是什麼？→ n ≥ 30；central limit theorem。
12. ASES 的 MCID 範圍？→ 依診斷與治療不同，約 6.4 到超過 17 分。

---

*本頁為兩版原文逐段比對後以中文自行整理的差異重點，非原文翻譯；數值以 OKU 15 原書為準。*
