# 使用嵌入式虛擬機
如果勾選了Virtualized Intel VT-x/EPT 而無法運行  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/v1.png)   
## 出現  Virtualized Intel VT-x/EPT is not supported on this platform 的錯誤   
1. 去BIOS看 有沒有開啟虛擬化  可以打開工作管理員 > 效能 > CPU > 看模擬有沒有啟用  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/v3.png)   
2. 去控制台 > 程式集 > 程式和功能 > 開啟或關閉Windows功能 > 把windows子系統Linux版 勾選 並重開機  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/v2.png)  
3. 在打開windows 安全性 > 裝置安全性 > 核心隔離詳細資料 >  把記憶體完整性取消勾選再重開機 就可以運行了  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/v4.png)   
以上是win 11 的做法  
win10 的第三步要去 把虛擬機的安全性用掉 要用本機群組原則編輯器修改(gpedit.msc)  
