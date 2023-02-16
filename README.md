# 2023 技術審查
評議職級: SPD4

[toc]

# Programming - level 3

### 重構 module level
<br>

|     | Specific  | Number  | Time  | prove |
|  ----  | ----  | ----  | ----  | ----  |
| 獨立網址重建 | 1. 舊有的獨立網址系統架構不適合加入新平台或功能，且程式框架較為複雜，因此重構<br> 2. 使用 React 和 golang 進行系統重構<br> 3. 以訂閱推播的方式推送資料 | 馬拉松 | 2022/09 ~ now |[issue](https://proton.vir000.com/castle/carriage/-/issues/9)|
| 抗劫持  | 原先抗劫持`單一`、`全部`地區的 IP 替換是透過存放在 Redis 資料庫做替換，透過將資料源<br>切換成 loki 的方式改善`資料保留與查詢不方便`、`檢測結果顯示不完整`、`檢測結果不即時`等問題| 2-3 member |2 sprint|[issue](https://proton.vir000.com/prediction/predictor/-/issues/388)|
|外部抗封鎖| 導轉規則驗證邏輯複雜，且複用性較高，透過模塊的抽離能更好的進行測試 | 1 member | 1 sprint |[code](https://proton.vir000.com/prediction/spiker/-/blob/157fb7f98995174e1d6ed3e96006741147c86e7e/src/Component/Redirection/RedirectionRuleValidation.js)|
<br>

<br>

### 必要時能夠與部門進行分享
<br>

|     | Specific  | Number  | Time  | prove |
|  ----  | ----  | ----  | ----  | ----  |
| Typescript| 1. 較為熱門<br> 2. 前端套件都以 TS 編寫<br> 3. 有實作經驗  | once | 20mis | [TypeScript](https://proton.vir000.com/hello/scrummaster/-/issues/90#note_64471https://proton.vir000.com/Jason/jason_gao/-/blob/master/TypeSctip%E7%B0%A1%E4%BB%8B.md) |

<br>

### 能夠獨立完成任務
<br>

|     | Specific  | Number  | Time  | prove |
|  ----  | ----  | ----  | ----  | ----  |
| 建站管理 | TBI | own | 2021 | [maid](https://proton.vir000.com/castle/maid/-/merge_requests?scope=all&state=merged&author_username=Jason) |
| 抗封鎖/抗劫持 | TBI | own | 2022 | [prospect](https://proton.vir000.com/prediction/prospect/-/merge_requests?scope=all&state=merged&author_username=Jason)<br> [hight five](https://proton.vir000.com/prediction/high-five/-/merge_requests?scope=all&state=merged&author_username=Jason)<br> [predictor](https://proton.vir000.com/prediction/predictor/-/merge_requests?scope=all&state=merged&author_username=Jason)|
| 外部抗封鎖 | TBI | own | 2022 | [spiker](https://proton.vir000.com/prediction/spiker/-/merge_requests?scope=all&state=merged&author_username=Jason)<br> [hitter](https://proton.vir000.com/prediction/hitter/-/merge_requests?scope=all&state=merged&author_username=Jason) |
| 獨立網址 | TBI | own | 2022/09 ~ now | [jockey](https://proton.vir000.com/castle/jockey/-/merge_requests?scope=all&state=merged&author_username=Jason)<br> [carriage](https://proton.vir000.com/castle/carriage/-/merge_requests?scope=all&state=merged&author_username=Jason) |
| Navigation | 維運 | own | - | [navy-js](https://proton.vir000.com/navigation/navy-js/-/merge_requests?scope=all&state=merged&author_username=Jason) |
| 部署腳本 | 建立專案部署腳本 | own |  | [外部抗封鎖前端專案](https://proton.vir000.com/prediction/prelude/-/merge_requests/378/diffs)<br> [獨立網址前端專案](https://proton.vir000.com/castle/castle-deploy/-/merge_requests/505/diffs) |


<br>

### 了解軟體架構
<br>

- 傳統 MVC 架構 View 代表 Html+JS+CSS。
<br>
<img src="img/mvc_arc.png" width="500" hight="250"/>

- 前後端分離 MVC，View 成為 ViewModel，前端則透過各種框架，有效解耦。
<br>
<img src="img/mvc_arc1.png" width="500" hight="250"/>

- 前端功能逐漸複雜 Model、View、Controller 依賴性過高，難以測試。MVP 有效的解耦 Model 與 Controller 的依賴。
<br>
<img src="img/mvp.png" width="500" hight="250"/>

- MVVM 模式下 View 完全解耦 Model 和邏輯控制，透過 data binding 機制操作狀態。
<br>
<img src="img/mvvm.png" width="500" hight="250"/>

- Redux 狀態管理機制，提升狀態的可控性
<br>
<img src="img/redux.png" width="500" hight="250"/>

- backend clean architecture
<br>
<img src="img/clean_arc.png" width="500" hight="250"/>

</br>
</br>
</br>

# Testing - level 3
### 會使用 TDD
</br>

|     | Specific  | Number  | Time  | prove |
| ---- | ----  | ----  | ----  | ----  |
| 獨立網址 | 導轉規則格式驗證於開發前列舉紅燈案例和綠燈案例 | once  | 1 sprint  | [prove](https://proton.vir000.com/prediction/spiker/-/merge_requests/19/diffs#c3f416414686ec7b4686933ad5bbbeb06c912c07)  |

</br>

### 熟悉測試框架
- 前端測試框架 Jest
  - Unit test
  - End to End Testing

|     | Specific  | Number  | Time  | prove |
|  ----  | ----  | ----  | ----  | ----  |
| 抗封鎖/抗劫持 | 前端`單元測試/End to end`測試  | 20~30 merge request | 1 年 | [prospect](https://proton.vir000.com/prediction/prospect/-/merge_requests?author_username=Jason&page=3&scope=all&state=merged) |
| 獨立網址 | 前端`單元測試/End to end`測試  | 30~40 merge request | 5 個月 | [jockey](https://proton.vir000.com/castle/jockey/-/merge_requests?author_username=Jason&page=3&scope=all&state=merged) |
| 外部抗封鎖前後台 | 前端`單元測試/End to end`測試 | 20~30 merge request | 6 個月 | [spiker](https://proton.vir000.com/prediction/spiker/-/merge_requests?scope=all&state=merged&author_username=Jason)</br>[hitter](https://proton.vir000.com/prediction/hitter/-/merge_requests?author_username=Jason&page=2&scope=all&state=merged) |

- 後端測試框架 Golang Testify
  - Unit test

|     | Specific  | Number  | Time  | prove |
|  ----  | ----  | ----  | ----  | ----  |
| 抗封鎖/抗劫持 | 後端單元測試  | 5 merge request | 1 年 | [prospect](https://proton.vir000.com/prediction/high-five/-/merge_requests?scope=all&state=merged&author_username=Jason) |
| 獨立網址 | 後端單元測試 | 50~60 merge request | 5 個月 | [carriage](https://proton.vir000.com/castle/jockey/-/merge_requests?author_username=Jason&page=3&scope=all&state=merged) |
| 外部抗封鎖 | 後端單元測試 | 5~10 merge request | 2 個月 | [high-five-external](https://proton.vir000.com/prediction/high-five-external/-/merge_requests?scope=all&state=merged&author_username=Jason) |

<br>
<br>
<br>

# Infrastructure/DevOps - level 3

### 實作監控流程或機制
<br>

|     | Specific  | Number  | Time  | prove |
| ---- | ----  | ----  | ----  | ----  |
|  監控機制  | 將前端和後端服務掛載本機 docker 並透過，API 實現 error log 告警  | - | - | [Demo](https://proton.vir000.com/Jason/deploy_demo) |

<br>

### 實作 CI/CD 流程
<br>

|     | Specific  | Number  | Time  | prove |
| ---- | ----  | ----  | ----  | ----  |
|  frontend  | 前端 ci 運行 test、lint、build 並生成 artifacts | - | - | [Demo](https://proton.vir000.com/Jason/frontend_demo/-/blob/master/.gitlab-ci.yml)  |
|  backend  |  後端 ci 運行 test、lint、build 並生成 artifacts  | - | - | [Demo](https://proton.vir000.com/Jason/backend_demo/-/blob/master/.gitlab-ci.yml) |

<br>

### 排除系統問題的能力
<br>

|     | Specific  | Number  | Time  | prove |
| ---- | ----  | ----  | ----  | ----  |
|  Grafana  | loki、prometheus | - | - | [監控](https://docs.google.com/spreadsheets/d/1KePlr570QtYpLeUmIyIHZaccwMvWuG0zuiNyddIzO9o/edit#gid=1002729262) |

<br>
<br>
<br>

# Domain Knowledge - level 3

### 了解領域知識和部門內討論
<br>

|     | Specific  | Number  | Time  | prove |
| ---- | ----  | ----  | ----  | ----  |
| 獨立網址 | - | - | - | [Event Storming](https://app.diagrams.net/#G1YBMYnE5o_LJmbV64sB2EFz_FwLxI5paX)  |
| 抗封鎖外部 | - | - | - | [Event Storming](https://app.diagrams.net/#G1XQnkLaQzv_EuoCMN6Q1WocEdZKt5YTpU)  |

<br>

### 定義問題與 PO 討論
<br>

|     | Specific  | Number  | Time  | prove |
| ---- | ----  | ----  | ----  | ----  |
|  獨立網址  | 和 PO 討論訂閱機制  | - | - | <img src="img/sub.png" width="200" hight="100"/> |
|  獨立網址  | 和 PO 討論 google 登入流程  | - | - | [issue](https://proton.vir000.com/castle/carriage/-/issues/32)  |
|  抗封鎖  | 和 PO 討論 批次更新可能遇到的狀況  | - | - | [issue](https://proton.vir000.com/prediction/high-five/-/issues/71)  |

<br>
<br>
<br>

# Support - level 2
### 能夠獨立解決50%的問題，並對客戶做出正確的回應
<br>

|     | Specific  | Number  | Time  | prove |
| ---- | ----  | ----  | ----  | ----  |
| frontend | 前端問題 100% | - | - | - |
| 新人導師 | 前端教學  | - | - | - |

<br>
<br>
<br>

# Experience - level 3

|     | Specific  | Number  | Time  | prove |
| ---- | ----  | ----  | ----  | ----  |
|  Android APP - JAVA/Kotlin | 開發 | - | 1-2 年 | - |
|  Android/IOS APP - React Native  | 開發 | - | 2-3 年 | - |
|  Web Application - React  | 開發 | - | 1 年 | - |
|  Web Service - golang  | 開發  | - | 1 年 | - |
<br>

# Soft

### 能夠發現問題,分析複雜問題的解決方案
<br>

|     | Specific  | Number  | Time  | prove |
| ---- | ----  | ----  | ----  | ----  |
|    |   |   |   |   |

<br>
<br>

### 持續為產品/流程的改進做出貢獻
<br>

|     | Specific  | Number  | Time  | prove |
| ---- | ----  | ----  | ----  | ----  |
|  CI Cache 優化  | 專案原本沒有針對 node_module 進行緩存，以至於 CI Job 特別緩慢 | - | - | [merge request](https://proton.vir000.com/prediction/spiker/-/merge_requests/9) |

<br>
<br>

### 能夠負責完整交付，小項目到正式環境
<br>

|     | Specific  | Number  | Time  | prove |
| ---- | ----  | ----  | ----  | ----  |
| spiker | 使用 ansible 腳本部署 QA和正式站  | - | - | [spiker](https://proton.vir000.com/prediction/spiker/-/tags) |
| hitter | 使用 ansible 腳本部署 QA和正式站  | -  | - | [hitter](https://proton.vir000.com/prediction/hitter/-/tags) |
| Jockey | 使用 ansible 腳本部署 QA和正式站  | -  | - | [jockey](https://proton.vir000.com/castle/jockey/-/tags) |

<br>
<br>

### 獨立管理專案
<br>

|     | Specific  | Number  | Time  | prove |
| ---- | ----  | ----  | ----  | ----  |
|  Trinity  | 專案建置、功能開發、問題除錯、測試、部署 | - | now | [trinity](https://proton.vir000.com/hello/trinity) |
|  prospect | 功能開發、問題除錯、測試、部署 | - | now |[prospect](https://proton.vir000.com/prediction/prospect) |
|  Spiker  | 專案建置、功能開發、問題除錯、測試、部署  | - | now | [Spiker](https://proton.vir000.com/prediction/spiker) |
|  Hitter  | 專案建置、功能開發、問題除錯、測試、部署 | - | now | [Hitter](https://proton.vir000.com/prediction/hitter) |
|  Jockey  | 專案建置、功能開發、問題除錯、測試、部署  | - | now | [Jockey](https://proton.vir000.com/castle/jockey) |


<br>
<br>

### 在複雜環境中操作,只須少量監管
<br>

|     | Specific  | Number  | Time  | prove |
| ---- | ----  | ----  | ----  | ----  |
|    |   |   |   |   |

<br>
<br>

### 持續學習並分享給團隊成員
<br>

|     | Specific  | Number  | Time  | prove |
| ---- | ----  | ----  | ----  | ----  |
| 分享工具 | Testing Playground  | - | - | <img src="img/testing_p.png" width="500" hight="250"/>  |
| 分享工具 | GitHub Copilot  | - | - | - |
