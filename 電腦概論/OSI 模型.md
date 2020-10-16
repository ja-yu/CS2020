# OSI 模型
```
https://zh.wikipedia.org/wiki/OSI%E6%A8%A1%E5%9E%8B
```
```
開放式系統互聯模型(Open System Interconnection Model)
```
```
第7層 應用層（Application Layer）
提供為【應用軟體】而設的介面
例如：HTTP、HTTPS、FTP、Telnet、SSH、SMTP、POP3

第6層 表達層（Presentation Layer）
把【數據轉換】為能與接收者的系統格式相容並適合傳輸的格式

第5層 會議層（Session Layer）
負責在數據傳輸中【設定】和【維護】電腦網路中兩台電腦之間的【通訊連接】

第4層 傳輸層（Transport Layer）
把【傳輸表頭（TH）】加至數據以形成數據包。傳輸表頭包含了所使用的協定等傳送資訊
例如:傳輸控制協定（TCP）

第3層 網路層（Network Layer）
決定數據的【路徑選擇】和【轉寄】，將網路表頭（NH）加至數據包，以形成封包。網路表頭包含了網路資料
例如:網際網路協定（IP）

第2層 資料連結層（Data Link Layer）
負責【網路尋址】、【錯誤偵測】和【改錯】
當表頭和表尾被加至數據包時，會形成【資訊框（Data Frame）】
數據連結串列頭（DLH）是包含了實體位址和錯誤偵測及改錯的方法。數據連結串列尾（DLT）是一串指示數據包末端的字串
例如:乙太網、無線區域網路（Wi-Fi）和通用分組無線服務（GPRS）

第1層 實體層（Physical Layer）
在局部區域網路上傳送資料框（Data Frame），它負責管理電腦通訊裝置和網路媒體之間的互通
例如:針腳、電壓、線纜規範、集線器、中繼器、網卡、主機介面卡
```
