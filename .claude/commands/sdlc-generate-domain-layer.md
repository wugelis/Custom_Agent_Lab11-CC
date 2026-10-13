---
description: 依 use case、sequence 與 class diagram 設計，產生 .NET 10 Domain Layer class library 專案（C# 程式碼置於 ./src）
---

將目前的 use case 到 sequence 與 class diagram 的設計，產生一個 .NET 10 的 class library 的專案。

(1). 將所有的 C# 程式碼放在 ./src 目錄下
(2). ToRentalCar() 方法遵循 use case 到 sequence 的那 4 件事情（選擇車型、租用時間區間、並計算租金，與確認租車）
(3). 在 ToRentalCar() 方法中，程式碼中這 4 件事情，每行程式碼都必須撰寫註解
