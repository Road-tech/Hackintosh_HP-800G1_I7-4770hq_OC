![HP 800 G1](https://raw.githubusercontent.com/Road-tech/Hackintosh_HP-800G1_I7-4770hq_OC/main/hp_800_g1.png)

# Hackintosh for HP 800G1, 4770hq using Opencore and Support macOS Big Sur

**此EFI在[shidongfei2](https://github.com/shidongfei2)修改升级**

---

## 注意

**使用EFI前请务必自行补足三码(SSN,UUID,ROM)！！！**    

---

## 关于这台小主机

HP 800G1 DM，在Haswell时代的1L小主机里是很有特色的存在，不仅可以上魔改u，还支持M.2 NVME协议的2280。空间充裕还可以上个2.5寸硬盘和白果拆机卡。在当时（购入与2019年底）看来，不论是入坑macOS还是windows日常办公，这都是一个台很好玩且有性价比的小主机。

总结一下，这台机子的优势是：

1. 可以使用四代魔改移动的 CPU，比较低的价格就可以上 i7 八核（曾经）；
2. 支持NVME协议、 2280长度的M.2硬盘；
3. 同时还支持2.5寸Sata硬盘，总计可以安装两块硬盘；
4. 网卡使用 ngff 接口且空间充裕，可以搭配转接卡使用用上白果的拆机网卡，完美驱动；
5. 硬件保有量比较大，不用担心被JS涨价（曾经）；
6. 噪音意外的小；

当然放在现在已经不太有购买价值了。

---

## 硬件

|                     	| Specifications / 型号               	| Note / 备注	|
| ------------------- 	|:------------------------------------:	|:------------:	|
| Motherboard/主板:     	| HP 800 G1                         	|           	|
| CPU/处理器:           	| I7-4770hq                       		|           	|
| CPU Cooler/散热器:    	| 自带                              		|           	|
| Hard Drive/硬盘:      	| Toshiba RD500 256gb              		|           	|
| RAM/内存:             	| 协德 8G DDR3L 1600MHz X2          		|           	|
| Wireless Card/无线网卡:	| BCM94360CS2                      		| 苹果拆机卡     	|
| Tower Case/机箱:      	| 自带                                 	|           	|
| Power/电源:           	| 7.4/5.5mm 19v 90w DC power adapter 	|           	|

---

## 功能

### Work：

- 两个DP接口输出(1080p)  
- 所有的USB接口  
- Wi-Fi & Bluetooth  
- 3.5mm音频接口
- 机箱内置音响
- Airdrop  
- AirPlay  
- Continuity  
- 睡眠
- CPU变频

### Not working:

- VGA接口

### 未测试:

- 4k 输出
- 3.5mm麦克风输入 

---

## BIOS设定：

- Security -> VTd -> Disabled。 
- Storage -> Storage Options -> SATA Emulation > AHCI   

---

## 禁用CFG Lock & 设定DVMT pre-alloc到64M

需要一定动手能力，请参考[不刷BIOS修改AMI BIOS的方法（以CFG Lock为例）](https://www.bilibili.com/read/cv4646116/)

---

# Performance/展示

待上传

---

# Reference/参考

- https://github.com/shidongfei2/800g1
- https://github.com/zearp/OptiHack
- https://github.com/mingcheng/dell-optiplex-9020m-hackintosh
- https://www.bilibili.com/read/cv4646116/
