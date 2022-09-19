# 使用嵌入式虛擬機
如果勾選了Virtualized Intel VT-x/EPT 而無法運行  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/v1.png)   
出現  Virtualized Intel VT-x/EPT is not supported on this platform 的錯誤   
先去BIOS看 有沒有開啟虛擬化  可以打開工作管理員 > 效能 > CPU > 看模擬有沒有啟用  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/v3.png)   
去控制台 > 程式集 > 程式和功能 > 開啟或關閉Windows功能 > 把windows子系統Linux版 勾選 並重開機  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/v2.png)  
