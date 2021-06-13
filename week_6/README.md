# 第六堂：Vue Router

### 本週作業

- [第六週主線任務：建立路由表](https://rpg.hexschool.com/training/18/task?type=detail&id=184)


## 主線說明：

- 為什麼要用 CLI
- CLI 環境安裝與了解
- 路由介紹


### 為什麼要用 CLI

- 不需從零建構環境，幾個選項後快速開發
- 快速建立「應用服務」 -> 單頁式應用程式
    - Router 管理由後端轉為前端
- 整合性的工具，開發更容易
    - 從 CDN 改為 NPM 統一管理


### CLI 環境安裝與了解

- 手動建置
    - Babel
    - Router → **Use history mode for router? False**
    - CSS 預處理 → node sass
    - Linter → 請至少選一個：Airbnb 是最嚴格的，不熟悉的可以選另外兩個
- 新增專案，不保存預設

運行方式：

- serve：運行開發環境
- build：編譯程式碼並釋出

資料夾結構說明：

- public：公開的檔案資料夾，可以放入不會被編譯的內容，裡面除了 index.html 外，其他都是直接被搬移的
- src：主要的開發環境


### Vue Cli 介面介紹

安裝插件：
- Vue loading
- vue axios
- Bootstrap Sass

@import '~bootstrap/scss/bootstrap';

### 環境變數

[https://cli.vuejs.org/zh/guide/mode-and-env.html](https://cli.vuejs.org/zh/guide/mode-and-env.html)

1. 新增 .env 檔案
2. 加入變數，API 網址及 Path


### Router

說明：Vue Router 不一定要搭配 Cli

https://next.router.vuejs.org/

元件與頁面連結的關係表
- 路由是什麼
    - 路由表
- 路由結構配置 → 基本頁面結構配置
    - 配置 router 檔案
    - router-view
    - router-link 連結方式
- 準備路由架構表
- 巢狀路由 → 巢狀連結
- 動態路由 → 動態參數
- this.$router.push(), back()
- default link


示範開發


1. 請先定好完整路由架構
2. 將**路由配置對應所有頁面，開發順序：**
    1. 先開頁面檔案
    2. 撰寫路由配置
    3. 補上 router-link
- 前端頁面
    - 首頁 /
    - 產品 /products → 產品列表
    - 產品 /product/:id → 動態路由
    - 購物車 /cart
- 登入頁面 /login
- **需驗證頁面：管理者端頁面** /admin/ —> 巢狀路由
    - 產品 /products
    - 訂單列表 /orders
    - 優惠券... /coupons

路由架構
- 首頁
    - 產品列表
    - 產品單一頁面
    - 購物車
    - 結帳頁面...
- 登入
- 後台
    - 產品管理列表
    - 優惠券列表
    - 訂單列表

## 補充：pathMatch

404 頁面
https://next.router.vuejs.org/guide/migration/#removed-star-or-catch-all-routes


### 本週作業

- [第六週主線任務：建立路由表](https://rpg.hexschool.com/training/18/task?type=detail&id=184)

- 課後可參考章節：[Vue Router](https://courses.hexschool.com/courses/vue-2021/lectures/31862625)