# 論文概念架構與多維度關鍵字矩陣 (v1.0)

**工作題目：** 結構主題模型視角下的媒體再現：共諜案件之新聞框架動態分析  
**文件定位：** 核心研究問題 (RQs) 與假設 (Hs) 之概念展開、變數操作化與文獻檢索指引  
**更新日期：** 2026-09-17  

---

## 一、 研究概念心智圖 (Conceptual Framework & Mind Maps)

---

### 1.1 論文總體研究設計架構 (Macro Research Framework)

```mermaid
flowchart TD
    classDef root fill:#1e3a8a,stroke:#3b82f6,stroke-width:2px,color:#ffffff,font-size:16px,font-weight:bold;
    classDef pillar fill:#f1f5f9,stroke:#475569,stroke-width:2px,color:#0f172a,font-size:14px,font-weight:bold;
    classDef goal fill:#ecfdf5,stroke:#10b981,stroke-width:2px,color:#065f46,font-size:14px,font-weight:bold;

    Title["結構主題模型視角下的媒體再現：<br/>共諜案件之新聞框架動態分析"]:::root

    Title --> P1["【理論視角】<br/>框架理論 × 媒體再現 × 安全化理論"]:::pillar
    Title --> P2["【核心研究問題與假設】<br/>RQ1 (關注度) / RQ2 (主導框架) / H1-H3 (動態消長)"]:::pillar
    Title --> P3["【實證方法與操作化】<br/>STM 結構主題模型 (協變量: 媒體立場 + 事件階段)"]:::pillar
    
    P1 --> Goal["【實務貢獻】<br/>國軍新聞輿情主動應處 × 分階段危機傳播 × 保防反情報教育"]:::goal
    P2 --> Goal
    P3 --> Goal
```

---

### 1.2 核心研究問題與假設推演邏輯鏈 (RQs & Hypotheses Flow)

以簡潔直觀的「自變數 (IV) $\rightarrow$ 應變數 (DV)」路徑呈現研究問題與假設的檢驗關係：

```mermaid
flowchart LR
    classDef iv fill:#e0f2fe,stroke:#0284c7,stroke-width:2px,color:#0369a1,font-size:14px,font-weight:bold;
    classDef dv fill:#fef3c7,stroke:#d97706,stroke-width:2px,color:#92400e,font-size:14px,font-weight:bold;
    classDef rq fill:#f1f5f9,stroke:#64748b,stroke-width:1.5px,color:#0f172a,font-size:13px;

    subgraph IV ["自變數 (Independent Variables)"]
        IV1["媒體政治立場<br/>(偏綠 / 偏藍 / 中立)"]:::iv
        IV2["事件發展階段<br/>(偵查 → 起訴 → 判決)"]:::iv
    end

    subgraph DV ["應變數 (Dependent Variables)"]
        DV1["國安威脅框架盛行率<br/>(中共滲透 / 統戰威脅)"]:::dv
        DV2["司法程序框架盛行率<br/>(偵審進度 / 法條判決)"]:::dv
        DV3["議題新聞報導總量<br/>(公眾關注度)"]:::dv
    end

    IV1 -- "H1：偏綠顯著高於偏藍/中立" --> DV1
    IV1 -- "H2：中立顯著高於偏綠" --> DV2
    IV2 -- "H3：隨審理推進顯著上升" --> DV2
    IV2 -- "RQ1：生命週期報導量消長" --> DV3
```

> **RQ2（主導新聞框架）：** 透過 STM 結構主題模型從全文本語料中萃取潛在主題，歸納並命名出如上列 DV1（國安威脅）、DV2（司法程序）等核心代表性新聞框架。

#### 研究問題與假設檢驗對照表
| 編號 | 自變數 (IV) | 應變數 (DV) | 控制條件 | 預期實證方向 / 核心內涵 |
| :--- | :--- | :--- | :--- | :--- |
| **RQ1** | 事件發展階段 | 新聞報導總量 | 全媒體 | 檢驗新聞量隨「偵查 $\rightarrow$ 起訴 $\rightarrow$ 判決」之消長趨勢 |
| **RQ2** | 全文本語料庫 | 主題框架分布 | 文本特徵 | 萃取臺灣媒體建構之代表性新聞框架種類 |
| **H1** | 媒體政治立場 | 國安威脅框架盛行率 | 控制事件階段 | 偏綠媒體之盛行率顯著高於偏藍與中立媒體 |
| **H2** | 媒體政治立場 | 司法程序框架盛行率 | 控制事件階段 | 中立媒體之盛行率顯著高於偏綠媒體 |
| **H3** | 事件發展階段 | 司法程序框架盛行率 | 控制媒體立場 | 判決階段之框架盛行率顯著高於偵查階段 |


---

### 1.3 理論基礎與概念傳播機制 (Theoretical Integration)

```mermaid
flowchart TD
    classDef tbox fill:#f8fafc,stroke:#475569,stroke-width:1.5px,color:#0f172a,font-size:13px;
    classDef theader fill:#4338ca,stroke:#6366f1,stroke-width:2px,color:#ffffff,font-size:15px,font-weight:bold;

    T_Root["共諜案件之媒體再現與傳播機制"]:::theader

    T_Root --> F1["【框架理論 (Framing Theory)】<br/>• Entman (1993) 四大功能：界定、因果、道德、處方<br/>• 新聞媒介對共諜威脅的選擇性凸顯與框架競爭"]:::tbox
    
    T_Root --> F2["【媒體再現 (Media Representation)】<br/>• Hall (1997) 社會真實建構與符號化產製<br/>• 『內部叛徒 vs. 國防群體』之他者化 (Othering) 機制"]:::tbox

    T_Root --> F3["【安全化理論 (Securitization Theory)】<br/>• 哥本哈根學派 (Buzan et al., 1998)<br/>• 國安發語行為 (Speech Acts) 與急迫生存威脅建構<br/>• 司法常態化 vs. 安全化非常態手段之拉鋸"]:::tbox

    T_Root --> F4["【議題生命週期 (Issue-Attention Cycle)】<br/>• Downs (1972) 新聞注意力起伏節奏<br/>• 偵查(震驚爆發) → 起訴(定錨聚焦) → 判決(熱度衰退/定罪)"]:::tbox
```

---

### 1.4 結構主題模型 (STM) 實證流程與協變量配置

```mermaid
flowchart LR
    classDef step fill:#f0fdfa,stroke:#0d9488,stroke-width:2px,color:#134e4a,font-size:14px,font-weight:bold;
    classDef detail fill:#ffffff,stroke:#94a3b8,stroke-width:1.5px,color:#334155,font-size:12px;

    subgraph S1 ["步驟一：語料庫建置"]
        A1["蒐集特定共諜案新聞全文本<br/>(涵蓋跨光譜主流媒體)"]:::step
        A2["標記詮釋資料 (Metadata):<br/>• 發稿日期 (Date)<br/>• 媒體名稱與立場 (Media)<br/>• 案件發展階段 (Stage)"]:::detail
        A1 --> A2
    end

    subgraph S2 ["步驟二：NLP 前處理"]
        B1["繁體中文斷詞與清洗"]:::step
        B2["• 載入國防/國安專用詞典<br/>• 過濾無關停用詞與版頭<br/>• 排除過低詞頻詞彙"]:::detail
        B1 --> B2
    end

    subgraph S3 ["步驟三：STM 建模與診斷"]
        C1["執行結構主題模型"]:::step
        C2["• 協變量公式：<br/>  prevalence = ~ Media + Stage + s(Time)<br/>• 診斷：語意連貫性 vs. 獨特性<br/>• 專家質性賦予主題框架命名"]:::detail
        C1 --> C2
    end

    subgraph S4 ["步驟四：假設檢定與推論"]
        D1["estimateEffect 效應檢驗"]:::step
        D2["• 檢定媒體立場邊際效應 (H1, H2)<br/>• 檢定事件階段演變效應 (H3)<br/>• 繪製動態框架消長曲線圖"]:::detail
        D1 --> D2
    end

    S1 ==> S2 ==> S3 ==> S4
```

---

## 二、 多維度中英文關鍵字群 (Multidimensional Keyword Clusters)

為便於在國內外各大資料庫（Web of Science、Scopus、Google Scholar、臺灣博碩士論文加值系統、Airiti Library 華藝線上圖書館）進行系統性文獻回顧，將關鍵字依「理論、方法、研究客體、動態變數、實務應用」拆解為五大維度：

### 維度一：傳播與理論視角 (Theoretical Dimensions)
| 類別 | 中文關鍵字 | 英文關鍵字 (English Keywords) |
| :--- | :--- | :--- |
| **框架理論** | 框架理論、新聞框架、二次框架、框架效果、框架競逐 | Framing theory, News framing, Frame building, Frame competition, Second-level agenda setting |
| **媒體再現** | 媒體再現、社會建構、意識形態、他者化、象徵符號 | Media representation, Social construction of reality, Ideology, Othering, Symbolic representation |
| **安全化理論** | 安全化理論、哥本哈根學派、安全化發語行為、威脅建構 | Securitization theory, Copenhagen School, Securitizing speech acts, Threat construction, De-securitization |
| **議題動態** | 議題生命週期、議題設定、新聞週期、媒體關注度 | Issue-attention cycle, Agenda setting, News cycle, Media attention, Salience dynamics |

---

### 維度二：計算方法與文本探勘 (Methodological Dimensions)
| 類別 | 中文關鍵字 | 英文關鍵字 (English Keywords) |
| :--- | :--- | :--- |
| **主題模型** | 結構主題模型、主題模型、潛在狄利克雷分配、機率模型 | Structural Topic Model (STM), Topic modeling, Latent Dirichlet Allocation (LDA), Probabilistic topic models |
| **協變量與效應** | 協變量效應、主題盛行率、主題內容分布、語意連貫性 | Covariate analysis, Topic prevalence, Topic content, Semantic coherence, Exclusivity |
| **計算傳播學** | 計算傳播學、文本探勘、自然語言處理、繁體中文斷詞 | Computational communication, Text mining, Natural Language Processing (NLP), Chinese word segmentation |

---

### 維度三：研究客體與領域情境 (Core Domain & Empirical Object)
| 類別 | 中文關鍵字 | 英文關鍵字 (English Keywords) |
| :--- | :--- | :--- |
| **間諜與國安** | 共諜案、中共滲透、國家安全、反情報、保密防諜、軍事洩密 | Espionage, Chinese espionage, Chinese infiltration, National security, Counter-espionage, Counterintelligence, Military leak |
| **法律與規範** | 國家安全法、反滲透法、國家機密保護法、刑法外患罪 | National Security Act, Anti-Infiltration Act, Classified National Security Information Protection Act, Treason / Espionage offenses |
| **政治與地緣** | 兩岸關係、統戰、混合戰、認知作戰、灰色地帶威脅 | Cross-strait relations, United front, Hybrid warfare, Cognitive warfare, Gray-zone threat |

---

### 維度四：自變數、分期與動態特徵 (Variables & Longitudinal Dynamics)
| 類別 | 中文關鍵字 | 英文關鍵字 (English Keywords) |
| :--- | :--- | :--- |
| **媒體立場** | 媒體政治偏向、政治立場、黨派偏見、媒體偏見 | Media bias, Political slant, Ideological orientation, Media partisanship |
| **司法分期** | 偵查階段、羈押審理、起訴、審判、一審判決、三審定讞 | Investigation stage, Pretrial detention, Indictment, Judicial trial, Court verdict, Final judgment |
| **時間維度** | 時間序列分析、動態分析、縱貫面分析、演變趨勢 | Time series analysis, Dynamic framing, Longitudinal analysis, Temporal evolution |

---

### 維度五：國軍傳播與實務對策 (Military & Practical Dimensions)
| 類別 | 中文關鍵字 | 英文關鍵字 (English Keywords) |
| :--- | :--- | :--- |
| **軍事傳播** | 國防新聞、軍事傳播、政治作戰、軍事公共事務 | Defense journalism, Military communication, Political warfare, Military public affairs |
| **危機應變** | 戰略溝通、危機傳播、公眾信任、國防形象維護 | Strategic communication, Crisis communication, Public trust, Defense institutional image |

---

## 三、 資料庫檢索式推薦 (Boolean Search Strings)

### 1. 國際英文資料庫 (Web of Science / Scopus)
- **檢索主題：STM 方法應用於新聞框架與安全議題**
  ```text
  TS = (("Structural Topic Model" OR "structural topic modeling" OR "STM") 
        AND ("framing" OR "news frame" OR "media representation") 
        AND ("national security" OR "threat" OR "espionage" OR "intelligence" OR "trial"))
  ```
- **檢索主題：安全化與媒體報導之動態分析**
  ```text
  TS = (("securitization" OR "threat construction") 
        AND ("media" OR "journalism" OR "news") 
        AND ("China" OR "Taiwan" OR "cross-strait"))
  ```

### 2. 臺灣學術資料庫 (Airiti Library 華藝 / 臺灣博碩士論文知識加值系統)
- **檢索主題：結構主題模型之新聞與傳播應用**
  ```text
  ("結構主題模型" OR "STM" OR "主題模型") AND ("新聞" OR "框架" OR "媒體再現")
  ```
- **檢索主題：共諜與國安法制之媒體再現或輿論分析**
  ```text
  ("共諜" OR "國安法" OR "反滲透法" OR "滲透") AND ("新聞" OR "框架" OR "報導" OR "媒體再現")
  ```
- **檢索主題：國軍形象、保防與軍事新聞傳播**
  ```text
  ("國防" OR "國軍" OR "軍事新聞") AND ("媒體再現" OR "形象" OR "危機傳播" OR "框架")
  ```

---

## 四、 核心研究問題與假設之操作化與診斷建議

為確保在 **11 月中旬計畫書口試** 能通過嚴格檢驗，針對現有 RQs 與 Hs 提出以下操作化微調建議：

### 1. 避免在假設中過早固化主題編號（如 T2、T4）
- **現象：** `PROJECT.md` 中寫道「偏綠立場媒體使用強調『中共滲透』等相關框架（對應 T2）」、「司法程序等相關框架（對應 T4）」。
- **建議：** STM 屬於非監督/半監督模型，主題編號（$K=1, 2, \dots$）是在模型訓練後隨機生成的。在第一階段假設提出時，應以**「概念框架名稱」**（例如「國安威脅框架」、「司法程序框架」）撰寫；待 Chapter 3 & 4 跑出主題並進行質性驗證標籤化後，再對應到特定主題編號，避免口試委員質疑「未跑模型先預設編號」。

### 2. 明確界定自變數（媒體政治立場）的分類指標
- **現象：** H1 比較「偏綠 vs. 偏藍/中立」，H2 比較「中立 vs. 偏綠」。
- **建議：** 
  1. 口試委員必定會詢問「偏綠、偏藍、中立」是以何種客觀標準界定（例如：引用傳播學界現有量表、報紙社論立場文獻、或是公視/中央社作為基準組）。
  2. 補足 H2 中「偏藍媒體」的假設位置：偏藍媒體在共諜案司法程序中是更偏向法律條文，還是聚焦於政治追殺/司法中立性質疑？

### 3. 事件生命週期之切點操作化 (RQ1 & H3)
- **建議：** 必須在研究設計中訂出「偵查、起訴、判決」三大階段的時間戳記（Timestamp）錨定規則（如：偵辦約談/羈押日、檢方起訴記者會日、法院宣判日）。這三個時間點將成為 STM 協變量中分段時間變數的核心。

---

## 五、 建議下一步行動 (Next Actions)

1. **文獻庫建立：** 利用上述檢索式，在 `01_papers/` 蒐集 8-12 篇核心文獻（特別是使用 STM 分析新聞框架之 SSCI/TSSCI 論文）。
2. **選案界定：** 具體選定 1-2 起指標性共諜案件（如退役將領案、現役軍士官滲透案），定義蒐集的時間跨度。
3. **自訂字典建置：** 著手規畫國防與共諜專有名詞清單，為後續 STM 斷詞前處理做準備。

