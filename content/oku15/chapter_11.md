---
title: "OKU 15 Ch.11: New Technology — Artificial Intelligence and Machine Learning（OKU 14 CH11 拆分）"
date: 2026-11-25
draft: false
tags: ["OKU15", "General Topics", "Artificial Intelligence", "版本差異"]
categories: ["OKU 15 更新"]
weight: 11
summary: "由 OKU 14 CH11 拆出的 AI／ML 章（16 頁）。重心從影像辨識與植入物辨識，轉向 LLM 病人端應用（ED 諮詢、衛教改寫、AI scribe）、care management／supply chain、OsteoSight 機會性骨質篩檢、AI + FEA／3D 列印客製設計，以及倫理（XAI、federated learning、偏誤、責任歸屬）。"
---

> **對照：**OKU 14 [CH11 New Technology（Robotics, AI, ML）]({{< relref "/chapter_11.md" >}}) 第 5 節 → OKU 15 **Ch.11**；機器人與 AR 另成 [Ch.10]({{< relref "/oku15/chapter_10.md" >}})｜作者群全新｜PDF 16 頁
>
> **閱讀方式：**🆕 新增；🔄 改變；✅ 一致；❌ OKU 15 不再涵蓋。這章以觀念為主，數據多是單一研究，考題多半考應用的方向與限制。

## 0. 考點變更總表

| 主題 | OKU 14 CH11 | OKU 15 Ch.11 | 類型 |
|---|---|---|---|
| 章節定位 | AI 是新技術章裡的一節 | 獨立成章，以「AI 涵蓋整個照護流程的閉環生態系」為主軸 | 🔄 |
| AI 的定義與分類 | AI、ML、DL 的定義；三類系統（intelligent algorithm、knowledge-based、neural network） | 改從**歷史脈絡**談：Turing test（1950）、**Dartmouth 會議（1956）正式提出 AI 一詞**、expert systems、Deep Blue（1997）、深度學習（2010 年代）、LLM | 🔄 |
| 影像應用 | 骨折、OA 分級、腫瘤、**植入物辨識**（多項 CNN 研究） | 骨折偵測（**scaphoid 漏診 > 30%，AI 偵測可達 96%**）、**AI-based RSA**、AI 加 FEA；植入物辨識研究**不再列出** | 🔄 |
| 病人端 LLM 應用 | 未提 | ChatGPT-4.0 做 ED 骨科諮詢，**不劣於、常優於專科醫師**；衛教改寫；AI scribe | 🆕 |
| NLP | Dragon Ambient eXperience；即時病歷與指令辨識 | 改舉 **AI scribe（Suki）**的數據：準確度與人工 scribe 相當，**每次看診省 60 秒** | 🔄 |
| Care management、supply chain | Bundled payment 的成本概念 | 自動 templating、**預測植入物需求**以減少庫存；CMS **CJR model** | 🆕 |
| 骨質疏鬆篩檢 | 未提 | **OsteoSight**：從一般 X 光機會性評估骨密度（**FDA Breakthrough Device**）；**Prognost** 預測骨折風險 | 🆕 |
| 個人化設計 | 未提 | AI 加 **FEA** 加 **3D printing** 設計客製植入物 | 🆕 |
| 倫理與限制 | 簡短的挑戰與結論 | 獨立成節：**XAI、black box、algorithmic bias、federated learning**、資料取得、責任歸屬、單向系統 | 🔄 |
| Navigation 的教訓 | — | **Navigation 在常規 arthroplasty 已被淘汰**：結果沒有比較好，又增加時間、成本和流程負擔，作為 AI 導入的警惕 | 🆕 |

---

## 1. 背景：骨科為什麼是「科技晚開花」🆕
- 骨科擅長機械方面的創新（不鏽鋼與鈦合金、UHMWPE、**1958 年 AO Foundation** 標準化內固定），但數位轉型很慢。
- **Navigation 的教訓：**1990 年代末出現 CT-based pedicle screw 導航與 CAS-TKA，但在一般 arthroplasty 從未普及。原因是**結果沒有優於傳統、增加時間與成本、打亂流程**，作者認為它在常規 arthroplasty **已經被淘汰**。
- 作者認為現在的機器人很多只是「導航加上機械手臂」，很少有即時數據分析或自適應學習，算不上真正的 AI。

## 2. AI 簡史（觀念題）
| 年代 | 里程碑 |
|---|---|
| 1950 | Turing 發表 *Computing Machinery and Intelligence*，提出 **Turing test** |
| **1956** | **Dartmouth 會議正式提出「artificial intelligence」一詞**，被視為 AI 研究的起點 |
| 早期 | Logic Theorist（定理證明）、Samuel 的跳棋程式（最早展示 machine learning） |
| 1980 年代 | **Expert systems**（rule-based） |
| 1990 年代 | 統計式 machine learning；**1997 年 Deep Blue 擊敗 Kasparov** |
| 2010 年代 | **Deep learning** 在影像與語音辨識上突破 |
| 近十年 | LLM（如 ChatGPT）進入日常使用 |

## 3. 醫學中的 AI 範例 🆕
- **Sepsis 早期預警演算法：**sensitivity 和 specificity 都是 0.87，**比臨床判斷提早 12 小時**預測惡化，準確度比單靠醫師好 32%，偽陽性減少 17%。
- 腫瘤學：預測基因型與治療反應，減少無效的昂貴療法。
- 病理學：不需要特殊染色就能辨識細胞型態。

## 4. 骨科影像與工程 🔄
- **骨折偵測：**scaphoid、部分 distal radius、femoral neck 骨折容易漏看。**Scaphoid 骨折漏診率超過 30%，AI 偵測率最高可達 96%。**
- **RSA（radiostereometric analysis）** 🆕：目前是**量測植入物 migration 和 wear 的標準**，做法是在植入物和組織內放 beads。**AI-based RSA** 與 model-based RSA 一致性良好，而且因為自動化，沒有觀察者之間的差異，**一致性更高**（THA 30 例）。
- **FEA（finite element analysis）**：模擬骨頭和植入物在負重下的力學反應。AI 可以自動建模、提高準確度，也能從影像預測骨強度和骨折風險。
- **Trauma 與 ICU：**以 MIMIC-III 的 2,662 位重症病人建立 30 天死亡率模型，**AUC 0.974**，已公開上線。
- **Registry 加 PROs：**CMS 的 **CJR（Comprehensive Care for Joint Replacement）model** 要求追蹤結果，AI 可以預測哪些病人可能達不到門檻。

> **OKU 14 的植入物辨識研究**（CNN 辨識 THA 和 TKA 元件、0.06 秒、100% 準確度等）在 OKU 15 **不再列出** ❌。

## 5. 病人端 AI 🆕（新版重點）
- **ED 諮詢：**2025 年研究中，**ChatGPT-4.0** 處理 ankle fracture、distal radius fracture、septic arthritis 等 ED 骨科情境，在完整性、幫助程度、具體性、整體品質上**不劣於、常常優於**專科醫師。在**病人衛教（counseling）**這一項，五種情境都由 AI 勝出。
- LLM 的診斷準確度也被報告**優於急診住院醫師**。
- **衛教文件改寫：**25 家醫學中心的衛教資料經 AI 改寫後，**閱讀年級下降 4.33 級，字數減少 442 字**。脊椎側彎術後的 FAQ，高二以上程度即可理解。
- **初診篩選：**作者的初步資料顯示，AI 問卷預測髖、膝痛病人是否為手術候選人的準確度約 **80–90%**。
- **AI scribe（Suki）：**194 次看診中，準確度與人工 scribe 相當，但精簡度和醫學用語較差。**新病人**（以病史為主）表現相當，**術後回診**（需要理學檢查和查閱舊病歷）表現較差。**每次看診省 60 秒，忙碌的 arthroplasty 醫師每天最多可省約 50 分鐘。**
- **風險：**AI 仍可能產生錯誤或虛構的內容（hallucination），必須查證。

## 6. Care management 與 supply chain 🆕
- **Advanced Case Management**：結合排程與病人資料，**自動 templating**，從術前影像**預測病人需要的植入物尺寸**。
- 好處：減少庫存、運輸與儲存，降低過期或淘汰的風險，加快手術室周轉。
- **OsteoSight**：從**一般 X 光機會性評估骨密度**，不需要額外檢查或轉介，已取得 **FDA Breakthrough Device designation**。
- **Prognost**：整合族群影像與臨床指標，預測骨折風險，優化骨質疏鬆處置。
- Registry 結合 EHR：持續監測，當併發症率或植入物表現偏離預期時提出警示。

## 7. AI 驅動的個人化設計 🆕
- AI 分析影像與結果資料，預測最適合的植入物幾何與材料。
- **FEA 是客製植入物上市前評估的關鍵**，可以減少實體原型測試，對翻修和特殊解剖特別有用。
- AI 結合 FEA 可以優化材料分布，**減少 stress shielding、促進 bone ingrowth**。
- **AI 結合 3D printing**：做出完全符合解剖的植入物或器械。
- 挑戰：法規、標準化流程、跨領域合作，以及長期生物相容性的驗證。

## 8. 倫理、風險與限制 🔄（高頻觀念）

| 問題 | 說明 | 解方 |
|---|---|---|
| **Black box** | 決策過程不透明，醫師難以信任 | **XAI（explainable AI）** |
| **Algorithmic bias** | 訓練資料缺乏代表性，造成不同族群的診斷與建議有差異 | 多元化的訓練資料、持續監測、嚴格驗證 |
| **資料取得受限** | 高品質資料被困在機構防火牆或付費牆後 | 推動開放資料，同時保護隱私 |
| **隱私與資安** | 集中式資料有外洩風險 | **Federated learning**：資料留在各醫院，只交換模型更新，符合 HIPAA |
| **責任歸屬** | AI 建議造成不良結果時，誰要負責仍不明確 | 建立法規框架 |
| **單向、靜態系統** | 只給建議，不接受使用者回饋；要重新寫程式才能更新 | 加入回饋迴路的 adaptive learning |

> **核心觀念：**AI 的目標**不是取代外科醫師，而是增強醫師的能力**，就像當年影像學改變了骨科一樣。

---

## 9. OKU 14 CH11 中 OKU 15 不再涵蓋的內容 ❌
- AI 的三類系統分類（intelligent algorithm、knowledge-based、neural network-based）
- 從 X 光辨識植入物的多項 CNN 研究
- Dragon Ambient eXperience 等 NLP 產品介紹
- Bundled payment 的成本分析段落

---

## 10. Anki 候選題

1. 「Artificial intelligence」一詞在哪一年、哪個場合首次提出？→ 1956 年 Dartmouth 會議。
2. Navigation 為什麼在常規 arthroplasty 被淘汰？→ 結果沒有比較好，又增加時間、成本與流程負擔。
3. Scaphoid 骨折的漏診率？AI 的偵測率？→ 漏診率超過 30%；AI 偵測率最高 96%。
4. 量測植入物 migration 和 wear 的標準方法？AI 帶來什麼改善？→ RSA；AI-based RSA 自動化、沒有觀察者差異，一致性更高。
5. ChatGPT-4.0 擔任 ED 骨科諮詢時，哪一項表現在所有情境都優於專科醫師？→ 病人衛教（counseling）。
6. AI 改寫衛教文件的效果？→ 閱讀年級下降約 4 級，字數減少約 440 字。
7. AI scribe 在哪一種門診表現較差？為什麼？→ 術後回診，因為需要理學檢查和查閱舊病歷。
8. 從一般 X 光機會性評估骨密度的 AI 工具？→ OsteoSight（FDA Breakthrough Device）。
9. 在不集中資料的情況下跨機構訓練 AI 的方法？→ Federated learning。
10. 解決 black box 問題的方向？→ Explainable AI（XAI）。
11. AI 結合 FEA 在植入物設計上的目標？→ 減少 stress shielding、促進 bone ingrowth。

---

*本頁為兩版原文逐段比對後以中文自行整理的差異重點，非原文翻譯；數值以 OKU 15 原書為準。*
