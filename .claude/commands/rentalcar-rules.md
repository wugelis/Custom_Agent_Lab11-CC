---
description: 租車系統業務規則說明
---

這是一個提供租車用戶可在線上預先租用車輛的系統。系統功能為，租車用戶可以在線上預約租車，而在租用車輛之前，租車用戶必須先註冊自已的帳戶資料後，並進行登入後才可預先租用車輛。在租用車輛時，可以選擇車型、租用時間區間、並計算租金，與確認租車這 4 件事情。

## Sequence Diagram 設計規則
租車用戶可進行線上租車，然而 (租車用戶/Actor) 需呼叫 ToRentalCar() 方法線上租用車輛，且選擇車型、租用時間區間、並計算租金，與確認租車這 4 件事情包含在 ToRentalCar() 這個方法裡面。


而且，在租用車輛之前，得先對 Account 領域物件 呼叫註冊帳號 RegisterAccount() 的方法。


## Class Diagram 設計原則
類別途中的 Domain Object 名稱與數量與 Sequence Diagram 完全相同。
Class 要實作哪些 Methods 由 Sequence Diagram 裡的 message 來決定。