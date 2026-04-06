# [Python Socket Programming]

## Proposal Report

### 動機與目標
<!-- 說明為什麼想做這個專題 -->
這個學期，我選修了電機系所開設的電腦網路導論選修課程，課程中介紹了 ISO/OSI 7層模型，並且提及了 socket 的實作。藉此機會，我想嘗試在 vs code 用 python 實作 socket，同時深入對 transport layer 以及資料結構與演算法的理解。

### 預期功能
<!-- 列出預計實作的功能 -->
1. 做出 socket 的基本架構，能夠讓 server 接收到 client 的 message。
2. 讓 client 與 client 之間能傳送訊息。
3. 視實作情況新增其他功能

### 使用技術
<!-- 使用的語言、框架、工具等 -->
在 vs code 上使用 python 進行實作。

### 時程規劃
<!-- 各週預計完成的進度 -->
1. 第十周完成 client-server 基本架構
2. 第十二周完成 client 之間的訊息交流

### 與課程的關聯
<!-- 你的專題可能涉及哪些資料結構或演算法概念？為什麼？ -->
在資料結構上，系統會使用緩衝區（通常以陣列或環形佇列實作）來暫存傳輸中的資料，並以佇列（queue）管理待處理的連線請求（例如 TCP 的 backlog queue）。在演算法方面，socket 通訊依賴網路協定（e.g. TCP）中的流量控制與擁塞控制演算法（Sliding Window），確保資料可靠且有效率地傳輸。

---

## Prototype Report

### 目前進度
<!-- 完成了什麼 -->
做出 socket 的基本架構，能夠讓 server 接收到 client 的 message。

### 遇到的困難
<!-- 遇到什麼問題、如何解決或打算如何解決 -->
在 cmd 執行的 client 端無法與 vs code 上的 server 端連接。經過多次檢查 client & server 的程式碼之後，發現問題出在沒有在電腦下載 python ，因此 cmd 無法執行 client code。

### 下一步計畫
<!-- 接下來要做什麼 -->
完成 client 之間的訊息交流。

### 與課程的關聯
<!-- 到目前為止，你的實作中哪些部分與課程內容有關？關係是什麼？ -->
對於 socket 之間資料訊息的傳送，格式需符合一定的 protocol(e.g. data size must no bigger than 64)，類似資料結構中，資料需要有一定組織的概念。
socket 的實作中，讓資料符合特定 protocol 要求的動作也算作一種 algorithm。

---

## Final Report

### 專案說明
<!-- 完整描述你的專案做了什麼 -->

### 使用方式
<!-- 如何編譯、執行、使用你的程式 -->

### 與課程的關聯總結
<!-- 總結你的專題與進階程式設計及資料結構課程之間的關聯 -->
