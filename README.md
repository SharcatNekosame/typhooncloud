#  颱風路徑運算 (Typhoon track computation)

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![Leaflet.js](https://img.shields.io/badge/Leaflet-199900?style=flat-square&logo=leaflet&logoColor=white)](https://leafletjs.com/)
[![CWA OpenData](https://img.shields.io/badge/CWA-OpenData-blue?style=flat-square)](https://opendata.cwa.gov.tw/)

這是一個結合**大氣科學開放資料（Open Data）**與**前端地圖互動技術**的颱風路徑運算系統。旨在透過視覺化介面，清晰呈現颱風的中心位置、歷史軌跡、未來預測路徑以及七級風暴風半徑，幫助使用者快速掌握氣象動態。

---

##  專案核心功能

1. **互動式網頁地圖視覺化 (Leaflet.js)**
   * 利用開源地圖框架，精準標繪颱風移動軌跡。
   * **圖層分離與色彩區分**：以不同顏色與樣式區分「當前中心點」、「歷史軌跡線（實線）」與「預測路徑（虛線）」。
   * **暴風圈半徑渲染**：透過圓形圖層（Circle）直觀展示預估七級風暴風範圍。
2. **智慧安全備案機制 (Fallback Mechanism)**
   * 考慮到方便更改參數的情況，內建預設**歷史颱風完整路徑備案（以 2026 年巴威颱風為例）**。
   * 能自動平滑切換至展示模式，確保介面完整性與展示效果。
3. **響應式設計 (RWD)**
   * 支援電腦與手機雙介面，左側固定資訊面板與右側全螢幕地圖配置，確保在各種尺寸螢幕上皆有良好的閱讀體驗。

---

## 技術架構與使用的工具

* **前端核心**：HTML5, CSS3, JavaScript (ES6+)
* **地圖圖資與互動**：[Leaflet.js](https://leafletjs.com/) (輕量級開源 JavaScript 地圖庫) + OpenStreetMap 圖資
* **資料來源**：交通部中央氣象署氣象資料開放平臺

---

## 專案畫面預覽

<img width="2559" height="1273" alt="image" src="https://github.com/user-attachments/assets/3dc4669a-1d79-4b58-a66e-8ad1d471e00d" />

---

##  如何執行此專案

本專案為純前端網頁，無需複雜的後端環境設定：

1. 將此專案複製到本機或直接下載：
   ```bash
   git clone [https://github.com/SharcatNekosame/typhoon.git](https://github.com/SharcatNekosame/typhoon.git)

   by.阮以樂
