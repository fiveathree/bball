# AI 籃球動作實驗室

上傳或拍攝籃球動作影片，用慢動作與逐格檢視拆解細節，在瀏覽器內做骨架分析，並與示範動作並排對照。

- 純靜態網頁，直接開 `index.html` 即可（建議經 localhost 或 HTTPS）。
- 影片及分析結果只存在你的瀏覽器（IndexedDB），不會上傳。骨架分析首次使用時需下載 MediaPipe 模型。
- 打開網頁即顯示一段側面拍攝的真人跳投示範片，與火柴人並排同步；上載自己的影片後會自動分析並同步。
- 請從側面拍攝，與示範火柴人同一角度才可對照；球員向左時火柴人會自動反轉。

目前功能：上傳／拍攝、慢動作、逐格、時間點筆記；六個動作的火柴人示範；骨架分析（身體、手部、臉部、籃球、關節角度、關鍵時刻）；真人片與示範並排同步。

## 第三方素材

- 示範片 `samples/jumpshot-side.mp4`：PNW Production，Pexels License。詳見 [samples/README.md](samples/README.md)。
- 骨架分析使用 [MediaPipe](https://ai.google.dev/edge/mediapipe)（Apache-2.0）及其預訓練模型。
