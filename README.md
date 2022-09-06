# cscio
## 配置
使用vmware,ultraVNC, wireshark  
使用pnet 虛擬機(記憶體跟核心 盡量越大越好)  
![GITHUB](https://github.com/timmy10289/cscio/blob/main/pictures/setting.png )    
進去之後可以登入root 密碼pnet(預設)  
![GITHUB](https://github.com/timmy10289/cscio/blob/main/pictures/setting2.png)  
第一次進去會要你在輸入密碼 一樣pnet(要輸入兩次) 之後再一直enter 就好了 不用輸入  
![GITHUB](https://github.com/timmy10289/cscio/blob/main/pictures/login.png)  
## 使用PNETLAB  
虛擬機開完就會有一個ip  (我這裡是192.168.239.128)  
![GITHUB](https://github.com/timmy10289/cscio/blob/main/pictures/setting3.png)  
輸入在自己的瀏覽器，最後再自己註冊或登入就可以了
![GITHUB](https://github.com/timmy10289/cscio/blob/main/pictures/loginpnet.png)  
## 元件下載
裡面有需要的東西  
https://drive.google.com/file/d/1CROJb8gxSrrKTYM3uLdnD1Xs9Va5qhT_/view?usp=sharing  
## 下載鏡像  
虛擬機登入後 打上 ifconfig | more  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/model2.png)  
記一下自己的ip  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/model3.png)  
去 putty 連線  (方便我們複製文字)  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/model4.png)  
帳號 root 密碼 pnet  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/model5.png)  
輸入 ishare search IOL  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/model6.png)  
選擇你要的鏡像 要一個L2 一個L3  找到就輸入 ishare pull 鏡像的名字 (不是每個都能下載，所以要一個一個試)   
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/model7.png)  
有成功的話 去看 PNETlab 有沒有冒出來L2 L3   就安裝完成  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/model8.png)  
## 正確關閉系統  
在左邊側欄按Setup Nodes 再按stop All Nodes  
![GITHIB](https://github.com/timmy10289/cisco/blob/main/pictures/stop1.png)  
在左邊側欄按 Destroy lab 再按destroy  
![GITHIB](https://github.com/timmy10289/cisco/blob/main/pictures/stop1.png)  
最後在虛擬機那邊 輸入 halt -p  就可以正確關閉虛擬機  
![GITHIB](https://github.com/timmy10289/cisco/blob/main/pictures/stop1.png)  

