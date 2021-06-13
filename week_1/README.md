# 第一堂：關注點分離

## Vue 作品實戰課程目標

- 掌握 Vue 3 技術
- 熟悉 JavaScript 實戰技巧
- 帶領每位同學完成「[屬於自己的獨立作品](https://works.hexschool.io/#/)」

## 課程專屬 API

本 API 將有助於學員完成屬於自己的獨立作品。

- 課程專屬 API：https://vue3-course-api.hexschool.io/
- API 文件：https://github.com/hexschool/vue3-course-api-wiki

## 課程學習說明

作業及挑戰
- 主線任務（**務必完成**）
- 分組任務
- 每日任務
- 支線任務

學習資源
- 錄影課程
- 直播課程
- 課程 API
- 額外課程練習講義
- Slack 學習頻道（主頻道、閒聊頻道、分組頻道）


## 本堂課程知識點

- 課程目標說明
- JavaScript 必學語法
- 關注點分離


### 1 JavaScript 必學語法

#### 縮寫形式

- 什麼是縮寫？什麼是新增語法？
- ES6 中必學的縮寫技巧

> 什麼時候會用到？撰寫程式碼都力求精簡、易於閱讀，縮寫正好符合此精神

#### 樣板字面值

- 可參考：[https://wcc723.github.io/javascript/2017/12/22/javascript-template-string/](https://wcc723.github.io/javascript/2017/12/22/javascript-template-string/)
    - HTML 結構換行更容易
    - 純文字中插入變數超簡單
- **樣板字面值技巧**
    - 知識點： `${}` 內可以帶入任何可回傳的結果

> 什麼時候會用到？撰寫程式碼都力求精簡、易於閱讀，樣板字面值概念亦同

#### 陣列方法

- forEach → 資料處理的技巧
    - 可參考：[https://wcc723.github.io/javascript/2017/06/29/es6-native-array/](https://wcc723.github.io/javascript/2017/06/29/es6-native-array/)
    - 只要會 forEach 就能吃全部
    - 進階技巧：輕鬆掌握 map, filter

> 什麼時候會用到？隨著資料處理日趨重要，各種陣列方法自然符合其需求

#### ESModule

- 關鍵點：如何匯出影響如何匯入
- ESMoudle 在實戰中的運用情境
    - 預設匯出：單一模組、元件開發
    - 具名匯出：函式庫、自訂方法集

> 什麼時候會用到？將程式碼模組化以及分類管理

### 2 關注點分離


- 相對於關注點分離，就是 “沒有關注點分離”
    - 資料跟畫面喇在一起
- 關注點分離，常見的分離點
    - HTML, JS 分離
    - 資料與方法分離
- 有哪些主流框架用到關注點分離：全部

案例：https://zh-hant.reactjs.org/docs/state-and-lifecycle.html
![](https://i.imgur.com/zUiOupA.png)

> 什麼時候會用到？前端框架、後端均是套用此概念，掌握對於未來學習及開發相當有幫助

#### 哪些可以被定義為 "data"

- 資料內容
- 狀態


#### 實戰演練

- 如何拆分資料
- 如何渲染畫面
- 如何重新取得資料
- 如何新增新的資料


---

## 第一週作業


* <a href="https://rpg.hexschool.com/training/18/task?type=detail&id=179" target="_top">第一週主線任務：關注點分離</a>


## 下週前預習章節

[錄影課程 API 串接說明](https://courses.hexschool.com/courses/vue-2021/lectures/32196753) -> 至少申請完 API Path