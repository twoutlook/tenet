---
layout: default
---
# 討論與決策



## 版本控制
- 持續使用 svn 或是改用 git?
- 服務器所在位置或租用服務?

## 開發工具
- 是否有計畫升級開發工具?
  - 台北直接使用VS2019,SZ仍使用VS2012。
  - 目前做法是台北組員以VS2019生成部署檔案,但在commit 到版本控制時,保持舊版的項目管控設定。


## 數據庫開發
- 和上項開發工具及項目配置有直接和間接的影響。
- 已知規格和限制
  - 是否升級現有 EF6 為 EF Core 的考慮,參考[微軟官網]([https://docs.microsoft.com/zh-tw/ef/efcore-and-ef6/)。

  
## WMS頁面應用
- 是否有計畫升級WMS頁面應用開發的底層框架?
- 已知規格和限制
  - 使用 WebForm, 參考[微軟官網](https://docs.microsoft.com/zh-tw/aspnet/web-forms/what-is-web-forms)。
  - 是否升級改用的考慮, 參考[微軟官網](https://docs.microsoft.com/zh-tw/dotnet/architecture/blazor-for-web-forms-developers/migration)。


## 權限平台
- 是否有計畫升級權限平台的機制和功能?
- NET 5 的標配
  - 使用Identity Server,參考[微軟官網](https://docs.microsoft.com/zh-tw/aspnet/core/blazor/security/webassembly/hosted-with-identity-server?view=aspnetcore-5.0&tabs=visual-studio)
  - Identity Server,參考[Identity Server 4 官網](https://identityserver4.readthedocs.io/en/latest/)



## WebPDA
- 是否有計畫升級目前的安卓應用的技術框架?
  - 是持續維持使用SZ的技術框架或是考慮啟用類似原生碼的開發模式?
    - 掃瞄功能是一個考量
    - 使用者友善介面是另一個考量
    - 安卓 apk 的定位是另一個考量
      - 面對TW客戶應考量安卓上架以顯示公司在這領域的專業定位。
- 已知規格和限制
  - 使用 WebView, 參考[微軟官網](https://developer.android.com/reference/android/webkit/WebView)。
  - 可以快速使用現有WEBPDA部署的網站,好像是安卓手機或PDA的應用。
    - PDA可以硬件操作啟用掃碼功能。
    - 手機無法啟用掃碼功能。必需在類似原生代碼的方式加入啟用照相功能才能掃碼。
