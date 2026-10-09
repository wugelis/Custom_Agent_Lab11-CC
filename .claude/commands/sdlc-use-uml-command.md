---
description: 從特定需求一次完成 Use Case Diagram、Sequence Diagram 到 Class Diagram 的 UML 建模
argument-hint: <需求描述>
---

請針對以下需求，依序完成 UML 建模，所有圖形一律使用 Mermaid 語法，並以 ```mermaid ``` 包裹於 Markdown 檔案中：

需求：$ARGUMENTS

若 $ARGUMENTS 為空，請參考專案根目錄的 README.md 作為需求來源。

## 執行步驟（必須依序執行，前一步的產出是下一步的輸入）

1. **Use Case 建模**：使用 `create-use-case-modeling` Skill，依需求的業務流程建立 Use Case Diagram，輸出為 `UC_<序號>_<系統名稱>.md`。
2. **Sequence Diagram**：使用 `create-sequence-diagram` Skill，依步驟 1 的 Use Case 與業務流程建立 Sequence Diagram，輸出為 `SD_<序號>_<系統名稱>.md`。
3. **Class Diagram**：使用 `create-class-diagram` Skill，依步驟 2 的 Sequence Diagram 找出領域物件 Domain Object，遵循 OMG UML 標準建立 Class Diagram，輸出為 `CD_<序號>_<系統名稱>.md`。

## 規則

- 檔名序號與系統名稱沿用專案既有檔案的命名慣例（例如 `UC_01_車輛租用系統.md`）。若檔案已存在，請先向我確認是否覆蓋。
- 三份圖形之間必須保持一致：Actor、Use Case、參與者與訊息、類別與方法名稱不可互相矛盾。
- 若專案有相關業務規則（如 rentalcar-rules、select-car-rules），請一併遵循。
- 全程以繁體中文回應。

## 完成後回報

列出三個產出檔案的路徑，並簡述各圖形涵蓋的重點，以及三者一致性的檢查結果。
