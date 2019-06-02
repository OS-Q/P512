# [KiCad](https://github.com/sochub/KiCad)

[![sites](SoC/qitas.png)](http://www.qitas.cn)

#### 硬件开发工具：[EDA](https://github.com/sochub/EDA)
#### 软件开发工具：[SDK](https://github.com/sochub/SDK)
### [KiCad简介](https://github.com/sochub/KiCad/wiki)

共享知识时代的发展注定通过开源淘汰不够进取的产品和利润十足的市场。传统的EDA巨头如[Cadence](https://github.com/sochub/Cadence)、[Altium Designer](https://github.com/sochub/Altium)、[mentor PADS](https://github.com/sochub/PADS)已是庞然大物，足以应付各种具有挑战性的设计，也是EDA行业发展的风向标，但如同硬件的发展一般，特别是智能硬件层面的简单PCB设计，在完全智能化程度不足的情况下提升产品的复杂度，很多强大的功能也只是屠龙之术，个人和中小型企业需要的也只是很简单的功能，所以更简单的EDA，而且没有成本的EDA是中小企业和创客群体的刚需。

在开源产品之前，国内学生和创客团体更多使用破解版本的[Altium Designer](https://github.com/sochub/Altium)软件上手实践，所以各种资源和库十分常见，学习入门也比较简单，但进入中大型企业可能就面临更换设计工具的问题，工作上使用的工具和个人平时使用的工具在一定程度上不统一，资源就会浪费，难免重复劳动，盗版软件毕竟是有心理障碍的。

KiCad于1992年由Jean-Pierre Charras在IUT de Grenoble工作时创建。2013年，CERN BE-CO-HT部门开始为KiCad提供资源，帮助促进KiCad与商用EDA工具相媲美。

版权声明：本文为博主原创文章，转载请附上博文链接！
[KiCad](http://kicad-pcb.org/) 是一款十分流行且强大的基于GPL的开源EDA，主要包括一个工程管理器和四个主要程序:

* kicad - 工程管理器
* eeschema - 原理图编辑器
* cvpcb - 元件封装关联选择器
* pcbnew - PCB布线程序
* gerbview - Gerber(光绘文件)查看器

pcbnew提供了至多50个层供电路板设计师使用：

* 32个铜层供导线走线（可覆铜）
* 14个固定用途技术层
    * 12个技术层对（上技术层和下技术层对称）
        * Adhesive, Solder Paste, Silk Screen, Solder Mask, Courtyard, Fabrication共计6对。
    * 2个独立技术层：Edge Cuts, Margin
* 4个辅助层可以任意使用：Comments, E.C.O. 1, E.C.O. 2, Drawings

Pcbnew的层描述中F.代表电路板上层（Front），B.代表电路板的下层（Back）

铜层是用于放置和重新布置导线的工作层。 层号从0开始（第一个铜层，在上层，即F.Cu），并以31（最后一个铜层，在下层，即B.Cu）结束。 由于元件不能放置在内层（层1到层30）中，所以只有层0（F.Cu）和层31（B.Cu）是元件层。

任何铜层的名字都是可以编辑的。层0的默认名称为F.Cu，层31的默认名称为B.Cu。当电路板是2层板时，层0和层31之间没有其他的铜层。当电路板是4层板时，层0和层31中间多了两个铜层，名称按从上层到下层的顺序依次为 In1.Cu 和 In2.Cu。当电路板是6层板时，层0和层31中间多了四个铜层，名称按从上层到下层的顺序依次为 In1.Cu，In2.Cu，In3.Cu 和 In4.Cu。

Adhesive (F.Adhes and B.Adhes)粘合层：用于在波峰焊前将SMD元件的粘合剂粘贴到电路板上的粘合层。

Solder Paste (F.Paste and B.Paste)焊膏层：在回流焊接之前生产掩模以允许焊膏放置在SMD元件的焊盘上。

Silk Screen (F.SilkS and B.SilkS)丝印层：元件图样标识的层，用于辅助元件的安装。

Solder Mask (F.Mask and B.Mask)阻焊层：定义了焊接的掩模，也就是不过绿油的区域。

Courtyard (F.CrtYd and B.CrtYd)空间层：用于显示元件在PCB上实际占用的空间大小。

Fabrication (F.Fab and B.Fab)生产层：用于辅助元件贴装。

### KiCad优点

* GPL开源软件，同时维护有大量开源资源
* 图形操作界面，鼠标和键盘操作很方便，支持脚本
* 相应功能全面，完全能够满足常规PCB的设计需求
* 跨平台的工具，linux、mac、windows都可以使用
* 可以直接生成gerber文件输出，不用担心文件格式

### KiCad特点

* 开源，便于硬件设计资料开源共享
* 软件不大，对电脑的配置要求不高
* 学习入门的门槛低，相关资料丰富
* 快捷键和热键强大，操作很人性化

### KiCad不足

* 相对常用的商业软件，功能不够完善，细节不够完美，如层管理，需要大量用到鼠标右键


###  [SoC资源平台](http://www.qitas.cn)

