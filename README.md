# WebReporter 基本資料

這是一個Web專案，用於提供報表服務，也可以往裡面添加Web API為其他程式提供服務

最初版使用Visual Studio Community 2019 搭配 .Net Core 2.2進行建置



## 版本信息

2019-07-17	Create by Ren

- [YG666] 提供出貨資料匯出EXCEL檔(台金庫)

2019-07-19	Modify by Ren	

- [YG666] 增加庫別選擇功能

2019-07-22	Modify by Ren

- [YG666] 1.增加模板選擇功能 2.完成亞源科技模板 3.新增輸入程式編號直達功能 4.將模板設置於檔案服務器方便更新 5. 前端UI調整

2019-07-23	Modify by Ren

- [Unity.DBProcess] 增加Database處理模塊，傳入sql及參數，返回DataTable或Dictionary<string, string>。

2019-07-24	Modify by Ren 

-	[_Layout.cshtml] 修改Bootstrap以及jQuery的引用路徑，以適應沒有Internet的環境。

2019-07-25	Modify by Ren	

- [YG666] 新增前端Bootstrap Alert提示錯誤信息、亞源科技報表誇庫邏輯修改
- [Unity.BootstrapAlert] 新增信息提示對象

2019-07-26	Modify by Ren

- [ZZ400] 新增ZZ-400加工二課標準包裝系統，完成前端畫面及前後端基本資料傳遞。

2019-07-30	Modify by Ren [YG666]

- 新增cxmr637通用方法，拷貝ERP的cxmr637邏輯。
- 新增KEP003A(康舒-1)以及KEP003W(康舒-W)

2019-07-31	Modify by Ren

- [YG666] KEP054A/B修正托數；新增KEU002A華隼
- [Unity.Convert] 新增周番6碼轉4碼功能

2019-08-02	Modify by Ren

- [YG666] 新增KEP004A/D東莞群光；修正DataGroupbyCustomerPN的箱數計算邏輯，改用cxmr637的資料加總。

2019-08-05	Modify by Ren

- [ZZ400] 完成ZZ400所有功能，圖片排列根據要求改成每行4個圖片，使用簡單爬蟲獲取客戶目錄下的所有圖片檔。

2019-08-06	Modify by Ren

- [Startup.cs] 增加啟動時的判斷以適應Linux服務器。

2019-08-08	Modify by Ren

- [YG666] 修正多角貿易如果單號對應錯誤，可能在對應料號時會跳不出while循環，涉及KEP003W、KEP054A/B

2019-08-09	Modify by Ren

- [JS600] 新增技術樣品資料EXCEL匯出。
- [YG666] 修正如果資料量小於2筆，部分模板插入空白欄位時會報錯的問題。

2019-08-12	Modify by Ren

- [JS600] 新增庫別選擇（金立、廣金）
- [YG666] 修正武漢康舒的多角貿易邏輯，避免同一個出貨日有多筆同一客戶的出貨單號時會導致取錯出貨單號。
- [API/ASFI] 新增MES團隊所需要的工單API，傳入工單號，返回JSON格式的資料。
- [Unity.DBProcess] 新增返回JSON格式之ResultJSON()方法，以ResultTable為基礎加工。

2019-08-15	Modify by Ren

- [JS600] 修正台金業務姓名獲取不到的問題
- [YG666] 根據要求修正武漢康舒ASN piece 改為托數

2019-08-20	Modify by Ren

- [YG666] 新增KED002C-重慶鴻富錦；KEP003P-菲律賓康舒

2019-08-21	Modify by Ren [YG666]

- 新增KEP060B-芬蘭賽爾康
- 修改調用DataGroupByCustomerPN()時順便把cxmr637的資料賦值至DataTable dtCxmr637
- 新增方法Convert_OGA01_TW2KL()用於把台金出貨單號轉換成金立的

2019-08-26	Modify by Ren

- [YG668] 新增YG668-嘜頭打印；新增模板KEP-002G光寶-PC

2019-08-27	Modify by Ren

- [YG667] 新增YG667-內外銷合併Packing List

2019-09-02	Modify by Ren

- [ZC200] 新增ZC200-資材備料計算

## 項目依賴

1. Excel操作
   - ClosedXML 0.94.2
2. Oracle資料庫操作
   - Oracle.ManagedDataAccess.Core 2.19.31
3. 網頁框架
   - ASP.NET Core 2.2.0
4. 反向代理服務
   - Nginx 1.16.0