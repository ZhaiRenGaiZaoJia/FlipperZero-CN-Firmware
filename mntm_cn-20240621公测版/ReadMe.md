20240621公测版更新日志：
-------------------------------------------------------------------------------------------
### 功能性重大更新

从该版本开始，汉化重点从汉化逐渐转向功能和用户体验的优化，在汉化的同时结合国人的使用习惯，对程序进行一定的修改和优化，目的是进一步降低用户的上手难度。


本次更新，系统性优化了NFC功能，汉化了所有与IC卡破解相关的程序，除了汉化以外，同时对程序进行了大量的修改，增加了操作引导提示和使用帮助，尽可能降低了上手的难度，优化了用户的体验。


#### 修改了系统NFC程序

针对使用字典进行初步解卡得到的文件，添加了卡片类型提示及相关引导说明，方便用户判断接下来该做什么。

<img src="screenshot/Screenshot-001.png">
<img src="screenshot/Screenshot-002.png">
<img src="screenshot/Screenshot-003.png">

优化先前汉化的同时增加了漏洞解卡选项，提示用户接下来都有哪些可用的解卡方式

<img src="screenshot/Screenshot-004.png">
<img src="screenshot/Screenshot-005.png">

#### NFC/Mifare Nested 嵌套认证攻击前置程序 1.6.5 (独立字库)

该程序是Mifare Classic (M1\S50\SAK08)卡Nested漏洞攻击的前置程序，作用是获取和收集攻击所需的随机数，汉化的同时增加了收集状态的显示，便于判断攻击方式，各种相关提示也进行了引导性的说明，同时在程序的帮助选项里增加了详细的功能及使用说明。该程序可以看作漏洞解卡的前置程序。

汉化的同时增加了收集状态的显示，便于判断攻击方式。

<img src="screenshot/Screenshot-006.png">
<img src="screenshot/Screenshot-007.png">

各种相关提示也进行了引导性的说明。

<img src="screenshot/Screenshot-008.png">
<img src="screenshot/Screenshot-009.png">

同时在程序的帮助选项里增加了详细的功能及使用说明。

<img src="screenshot/Screenshot-010.png">
<img src="screenshot/Screenshot-011.png">
<img src="screenshot/Screenshot-012.png">
<img src="screenshot/Screenshot-013.png">

#### NFC/MFKey 嵌套认证攻击程序 2.2 (独立字库)

该程序的作用是通过收集的随机数在本地模拟卡片然后遍历所有可能的密钥，该程序是利用卡漏洞在设备端解卡的核心程序程序，支持多种攻击方式的随机数破解。

<img src="screenshot/Screenshot-014.png">
<img src="screenshot/Screenshot-015.png">
<img src="screenshot/Screenshot-016.png">
<img src="screenshot/Screenshot-017.png">
<img src="screenshot/Screenshot-018.png">


也就是说小海豚除了字典和侦测，同样支持使用漏洞进行解卡，系统NFC程序搭配扩展程序中的Mifare Nested和MFKey程序，再配合电脑和手机，理论上至少可以解开市面上80%的IC卡(M1卡)。

之所以重点去搞了NFC功能，是因为小海豚的圈子里，长久以来的普遍共识是小海豚只支持字典攻击，不支持漏洞攻击，这让我很疑惑。毕竟侦测功能就摆在那里。通过深入了解和学习以后发现其实小海豚破解IC卡的能力非常强大，并非传闻中那样弱，只不过专业性较强罢了。而且由于支持多种类型的卡片，其用途在某些方面要强于部分专用复卡设备(毕竟大量复卡设备只能搞M1和EM4100卡)。

再加上其全开源，功能扩展方面也是潜力巨大，隔一段时间看看有什么新功能被折腾出来也是很有意思的一件事。


### 外部程序汉化：

#### 汉化Tools/RFID detector 读卡器类型检测 1.2 (独立字库)

该程序用于检测读卡器(读头)类型，可以很好的判断读卡器使用的是IC卡还是ID卡，同时还可以检测ID卡的具体频率。

<img src="screenshot/Screenshot-019.png">
<img src="screenshot/Screenshot-020.png">
