# 目標  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0920/goal2.png)  
新增三個路由器 (L3)  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0920/hw01.png)  
R1   en > conf t > hostname R1  
int e0/0 > ip addr 192.168.1.1 255.255.255.0 > no shut  
int e0/1 > ip addr 192.168.2.1 255.255.255.0 > no shut  
int lo1 > ip addr 1.1.1.1 255.255.255.0  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0920/hw02.png)  
R2   en > conf t > hostname R2  
int e0/0 > ip addr 192.168.2.2 255.255.255.0 > no shut  
int e0/1 > ip addr 192.168.3.2 255.255.255.0 > no shut  
int lo1 > ip addr 2.2.2.2 255.255.255.0  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0920/hw03.png)  
R3   en > conf t > hostname R3  
int e0/0 > ip addr 192.168.1.3 255.255.255.0 > no shut  
int e0/1 > ip addr 192.168.3.3 255.255.255.0 > no shut  
int lo1 > ip addr 3.3.3.3 255.255.255.0  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0920/hw04.png)  
R1  
ip route 2.2.2.0 255.255.255.0 192.168.2.2  
ip route 3.3.3.0 255.255.255.0 192.168.1.3  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0920/hw05.png)  
R2  
ip route 1.1.1.0 255.255.255.0 192.168.2.1  
ip route 3.3.3.0 255.255.255.0 192.168.3.3  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0920/hw06.png)  
R3  
ip route 1.1.1.0 255.255.255.0 192.168.1.1  
ip route 2.2.2.0 255.255.255.0 192.168.3.2  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0920/hw07.png)  
在R1     do ping 2.2.2.2 source 1.1.1.1   成功  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0920/hw08.png)  
do ping 3.3.3.3 source 1.1.1.1  成功  
![GITHUB](https://github.com/timmy10289/cisco/blob/main/pictures/0920/hw09.png)  
