![HP 800 G1](https://github.com/Road-tech/hp_800_g1_mini_hackintosh/blob/master/hp_800_g1.png?raw=true)

# Hackintosh for HP 800G1, 4770hq using Opencore and Support macOS Big Sur  

**此EFI在[shidongfei2](https://github.com/shidongfei2)修改升级**

---

## 注意

**使用EFI前请务必自行补足三码(SSN,UUID,ROM)！！！**    

---

## 关于这台小主机

HP 800G1 DM，在Haswell时代的1L小主机里是很有特色的存在，虽然比起同平台的联想（M73、M93）、戴尔（3020M，9020M）等的1L小主机丑了不少（PS.这个800G1看起来真的满满的年代感，很显旧），但是他很独特的选用了M.2接口而不是miniPCI。 而且相比起其他选用了M.2接口的小主机，他的M.2接口支持NVME协议（魔改后），而不是SATA协议。 虽然这个NVME协议速度并没有达到X4满速率，但是速度也比msata协议快不少。同时支持2280长度让硬盘的选择也很自由。 无线网卡的接口也是M.2且空间很充裕，可以轻松的通过转接卡用上白果的拆机网卡，不需要注入驱动就可以在macOS下实现隔空投送、接力、手表解锁等。 最后通过往BIOS注入微码可以使用如4980hq、4770hq等移动端魔改U，这类魔改u的4代i7，4c8t的配置，放在当时400左右的价格，性能并不会比同价位的6-8代的CPU（i3 8100之类）相差太多。 虽然4代CPU用的都是22nm工艺，会比14nm+++的工艺热不少，但是这类魔改u普遍搭载的是iris 5200核显，不仅黑苹果可以较完美的驱动，且性能要比祖传UHD630好不少（iris5200核显拥有40EU和128m的L4缓存，hd630仅24EU）。  综合以上数点，在当时（购入与2019年底）看来，不论是入坑macOS还是windows日常办公，这都是一个台很好玩且有性价比的小主机。

当然，放到现在已经是毫无性价比了。这台HP 800G1 DM我在19年底购入要360，4770hq魔改要420。而当时最便6代小主机要500+，最有性价比的ql2x好像也要480？（记不清楚了），所以在当时选择800G1还是有性价比的。到现在800G在tb还是这个价格，加上4代魔改i7全网没货，只剩下咸鱼传家宝开价500+。比起现在6代小主机比这个4代的800g1还便宜，而且还有神奇的6c12t的魔改8850H，只要450原。让这个800G1已经没有性价比了。没办法，谁叫我懒呢，折腾到现在才搞好macOS的安装。

总结一下，这台机子硬件方面的优势是：

1. 可以使用四代魔改移动的 CPU，比较低的价格就可以上 i7 八核（曾经）；
2. 支持NVME协议、 2280长度的M.2硬盘；
3. 同时还支持2.5寸Sata硬盘，总计可以安装两块硬盘；
4. 网卡使用 ngff 接口且空间充裕，可以搭配转接卡使用用上白果的拆机网卡，完美驱动；
5. 硬件保有量比较大，不用担心被JS涨价（曾经）；
6. 噪音意外的小；

## 硬件
|                     	| Specifications / 型号              	| Note / 备注  	|
| ---------------------	|:------------------------------------:	|:------------:	|
| Motherboard/主板:  	| HP 800 G1                        		|              	|
| CPU/处理器:           	| I7-4770hq                           	|            	|
| CPU Cooler/散热器:    	| 自带                   		        |            	|
| Hard Drive/硬盘:     	| Toshiba RD500 256gb          	        |            	|
| RAM/内存:            	| xiede 8G DDR3L 1600MHz X2         	|            	|
| Wireless Card/无线网卡:	| BCM94360CS2                   		| 苹果拆机卡  	|
| Tower Case/机箱:      	| 自带                                	|            	|
| Power/电源:           	| 7.4/5.5mm 19v 90w DC power adapter 	|            	|

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