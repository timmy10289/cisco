# HW
目標  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0913/hw.png)  
新增一台 VPC 像這樣連起來  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0913/hw01.png)  
打開 R1 > en > conf t > hostname R1 > int e0/1  進入e0/1  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0913/hw02.png)  
輸入 ip addr 192.168.2.254 255.255.255.0  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0913/hw03.png)  
no shut 開啟  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0913/hw04.png)  
end 結束編輯  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0913/hw05.png)  
sh ip int brief 觀察編輯結果  再輸入 conf t 進編輯  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0913/hw15.png)  
ip dhcp pool pool2  新增pool2  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0913/hw07.png)  
network 192.168.2.0 255.255.255.0  設定網路  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0913/hw08.png)  
default-router 192.168.2.254  設定路由  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0913/hw09.png)  
dns-server 8.8.8.8  設定dns  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0913/hw10.png)  
exit 回到上一層  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0913/hw11.png)  
ip dhcp excluded-address 192.168.2.1 192.168.2.99  排除1到99  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0913/hw12.png)  
ip dhcp excluded-address 192.168.2.201 192.168.2.254  排除201到254  就可以了  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0913/hw13.png)  
打開實驗機 ip dhcp  跟 show ip 分配網路  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0913/hw14.png)  
去ping 看看其他實驗機 有收到封包就是成功了  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0913/hw16.png)  
  
