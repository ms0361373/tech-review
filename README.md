## 技術審查

#### Programming
***
<br>

### 重構 module level
<br>

前端

|     | Specific  | Number  | Time  | prove |
|  ----  | ----  | ----  | ----  | ----  |
| 獨立網址| 一般登入替換 google 登入 | 1人 | 1 sprint | [issue](https://proton.vir000.com/castle/carriage/-/issues/32) |
|外部抗封鎖| 導轉規則驗證模塊抽離 | 1人 | 1 sprint |[code](https://proton.vir000.com/prediction/spiker/-/blob/157fb7f98995174e1d6ed3e96006741147c86e7e/src/Component/Redirection/RedirectionRuleValidation.js)|
<br>

後端
|     | Specific  | Number  | Time  | prove |
|  ----  | ----  | ----  | ----  | ----  |
| 抗劫持  | 重構檢測結果資料來源由 Redis 更換為 Loki | 2-3人 |2 sprint|[issue](https://proton.vir000.com/prediction/predictor/-/issues/388)|
| 獨立網址  | 獨立網址重建 |

***
<br>

### 必要時能夠與部門進行分享
<br>

|     | Specific  | Number  | Time  | prove |
|  ----  | ----  | ----  | ----  | ----  |
| Typescript| Typesciprt分享 | 1 次 | 20mis | [TypeScript](https://proton.vir000.com/hello/scrummaster/-/issues/90#note_64471https://proton.vir000.com/Jason/jason_gao/-/blob/master/TypeSctip%E7%B0%A1%E4%BB%8B.md) |

***
<br>

### 能夠獨立完成任務
<br>

|     | Specific  | Number  | Time  | prove |
|  ----  | ----  | ----  | ----  | ----  |
| 訂閱推播| 完成獨立網址推播/訂閱功能 | 1人 | 1 sprint | [訂閱推播](https://proton.vir000.com/castle/carriage/-/issues/17) |
| Google 登入 | 完成獨立網址 google 登入和權限控制 | 1人  | 1 sprint | [登入](https://proton.vir000.com/castle/carriage/-/issues/32) |

***
<br>

### 了解軟體架構
<br>



- 傳統 MVC
傳統 MVC 架構 View 代表 Html+JS+CSS
<br>
<img src="img/mvc_arc.png" width="500" hight="250"/>

- 前後端分離 MVC
<br>
<img src="img/mvc_arc1.png" width="500" hight="250"/>

- MVP
<br>
<img src="img/mvp.png" width="500" hight="250"/>

- MVVM
<br>
<img src="img/mvvm.png" width="500" hight="250"/>

- React + Redux
<br>
<img src="img/redux.png" width="500" hight="250"/>

- backend clean architecture
<br>
<img src="img/clean_arc.png" width="500" hight="250"/>


## Testing
### 會使用 TDD
- [前端](https://proton.vir000.com/prediction/spiker/-/merge_requests/19/diffs#c3f416414686ec7b4686933ad5bbbeb06c912c07)
***
### 熟悉測試框架
前端測試框架 Jest
- Unit test
- End to End Testing

|     | Specific  | Number  | Time  | prove |
|  ----  | ----  | ----  | ----  | ----  |
| 抗封鎖/抗劫持 | 前端`單元測試/End to end`測試  | 20~30 merge request | 1 年 | [prospect](https://proton.vir000.com/prediction/prospect) |
| 獨立網址 | 前端`單元測試/End to end`測試  | 30~40 merge request | 4 個月 | [jockey](https://proton.vir000.com/castle/jockey) |
| 外部抗封鎖前後台 | 前端`單元測試/End to end`測試 | 20~30 merge request | 4 個月 | [spiker](https://proton.vir000.com/prediction/outside-spiker)</br>[hitter](https://proton.vir000.com/prediction/outside-hitter) |

後端測試框架 Golang Testify
- Unit test

|     | Specific  | Number  | Time  | prove |
|  ----  | ----  | ----  | ----  | ----  |
| 獨立網址 | 後端單元測試 | 50~60 merge request | 4 個月 | [carriage](https://proton.vir000.com/castle/carriage) |
| 外部抗封鎖 | 後端單元測試 | 5~10 merge request | 4 個月 | [high-five-external](https://proton.vir000.com/prediction/high-five-external) |

***
## Infrastructure/DevOps

- [實作監控流程或機制](https://proton.vir000.com/Jason/deploy_demo)
- 排除系統問題的能力
    - Grafana
- 實作 CI/CD 流程
    - [前端](https://proton.vir000.com/Jason/frontend_demo)
    - [後端](https://proton.vir000.com/Jason/backend_demo)
***
## Domain Knowledge 6
Level 3
- [ ] 了解領域知識和部門內討論
    - [ ] 前端 (React)
    - [ ] 後端 (Golang)
    - [ ] 資料庫 (Mysql、Redis)
- [ ] 定義問題與 PO 討論
    - [ ] online issue 查找/討論
