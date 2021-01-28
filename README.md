# ProjectEvolution
## 一款航模/无人机/机器人遥控器  
### A RC/Drone/Robot Controler    
  
&emsp;本项目起始于2020年底，但追溯起来，我个人自制遥控器可以一直延伸到2016年左右。2015年由于资金和安全等原因，我放弃了自制火箭项目，转而玩多旋翼无人机，当时的大疆还是一颗争议不断的新星，Doby无人机正在火热众筹，我正即将从高中毕业，也正在自学Arduino。相比火箭，多旋翼使用成本几乎可以忽略不计，安全性也大大提高，但放在我眼前的第一件事就是遥控器的选择。  
&emsp;多旋翼无人机是从航模的基础上发展而来技术，因此当时大多数自制无人机也都采用成品航模遥控器，然而对于一个四线城市的农村高中生来说，即使是富斯i6也让我觉得太贵了，更何况越是便宜的遥控器，功能就越简陋，更难以让我这个轻度强迫症患者接受。既然好的买不起，买得起的又太渣，那干脆就自己做吧。我没有想到的是这个坑到现在我还没有填上，，，，，  
&emsp;我的第一套自制的遥控系统是在2016年暑假完成的，样子相当简陋，但还是用了模块化的设计，主控是Arduino nano，遥控器分为左右摇杆模块、显示模块、核心模块，可以组合成极简模式和完全体模式。  
 ![2016_1_01](https://github.com/liulizhi1031/ProjectEvolution/blob/master/Reference/PastProjectImages/2016_1_01.jpg)  
 ![2016_1_02](https://github.com/liulizhi1031/ProjectEvolution/blob/master/Reference/PastProjectImages/2016_1_02.jpg)  
 ![2016_1_03](https://github.com/liulizhi1031/ProjectEvolution/blob/master/Reference/PastProjectImages/2016_1_03.jpg)  
&emsp;2016年9月，我进入河北科技大学，成为飞行器设计与工程专业的首批学生，一个月以后我加入了电气学院409实验室（大学生创新素能基地）接着填我的坑。我使用了3块Arduino nano以满足功能需要，分别负责显示、数据读取、通信和数据处理。然而结果是惨烈的，Arduino孱弱的性能根本无法支撑如此的野心，只有STM32才能救项目！  
 ![2016_2_01](https://github.com/liulizhi1031/ProjectEvolution/blob/master/Reference/PastProjectImages/2016_2_01.jpg)   
 ![2016_2_02](https://github.com/liulizhi1031/ProjectEvolution/blob/master/Reference/PastProjectImages/2016_2_02.jpg)  
 ![2016_2_03](https://github.com/liulizhi1031/ProjectEvolution/blob/master/Reference/PastProjectImages/2016_2_03.jpg)  
 ![2016_2_04](https://github.com/liulizhi1031/ProjectEvolution/blob/master/Reference/PastProjectImages/2016_2_04.jpg)  
&emsp;接下来开始学习研究STM32，我发现F1和F4的学习难度几乎相同，因而直接上到STM32F407VET6，屏幕使用电阻触摸屏，然而做到一半我发现我的板子被焊成了假发，密密麻麻的飞线无不触发我的强迫症，因此学习PCB绘制看来是下一个必须解决的问题。  
 ![2017_1_01](https://github.com/liulizhi1031/ProjectEvolution/blob/master/Reference/PastProjectImages/2017_1_01.jpg)  
 ![2017_1_02](https://github.com/liulizhi1031/ProjectEvolution/blob/master/Reference/PastProjectImages/2017_1_02.jpg)   
 ![2017_1_03](https://github.com/liulizhi1031/ProjectEvolution/blob/master/Reference/PastProjectImages/2017_1_03.jpg)  
&emsp;与此同时我申报了大学生创新训练项目，虽然只拿到了校级，但顺便拿个名头也还不错了。由于此时我还在航模协会摸鱼，因此也学到了CAD和SolidWorks，接下来就是用STM32、AD、CAD来给这个项目做个了断了。虽然项目结了题，但是我对这套硬件并不满意，亚克力的外壳极为脆弱又搁手，体积虽然比我当时用的AT9小的多，但显然我馋了刚刚发布的大疆Mavic遥控器的身子，因此我又开启了新的征途。  
 ![2017_2_01](https://github.com/liulizhi1031/ProjectEvolution/blob/master/Reference/PastProjectImages/2017_2_01.jpg)  
 ![2017_2_02](https://github.com/liulizhi1031/ProjectEvolution/blob/master/Reference/PastProjectImages/2017_2_02.jpg)  
 ![2017_2_03](https://github.com/liulizhi1031/ProjectEvolution/blob/master/Reference/PastProjectImages/2017_2_03.jpg0)  
&emsp;这次为了更加紧凑，使用了游戏机摇杆（这显然是个致命缺陷），主控STM32F405RGT6直接贴在PCB上，屏幕也缩水到1.8寸（又一个致命缺陷）。一个偶然的机会我发现网上的3D打印服务还不错，而实验室申请的3D打印机一直久批不下，因而只能从网上找平台了，不得不说，光固化真香。总的来看，此时的遥控器和最初的遥控器早已天差地别，但距离成品和我的预期还差的远。  
 ![2018_01](https://github.com/liulizhi1031/ProjectEvolution/blob/master/Reference/PastProjectImages/2018_01.jpg)  
 ![2018_2020_1](https://github.com/liulizhi1031/ProjectEvolution/blob/master/Reference/PastProjectImages/2018_2020_1.JPG)  
&emsp;接下来的一年就是准备考研，但显然我高估了自己对考试的忍耐程度，直到2020年初，打着毕设的幌子，我重新开始填坑，这次希望能让遥控器更加成熟吧。毕设的进度催促着我要把重心向着多旋翼端偏移，这个控也仅仅完成了硬件的初步设计，软件更是只建了个文件夹。当然暴露的问题也不少，包括由于屏幕中置使遥控器过宽、过于集中化的PCB设计使试错成本猛增、握持手感极差等等一系列细节问题。  
 ![2018_2020_2](https://github.com/liulizhi1031/ProjectEvolution/blob/master/Reference/PastProjectImages/2018_2020_2.JPG0)  
&emsp;时间来到现在，2020年我一直在准备考研二战，一年的闭关修炼差点直接把我送走，还好这一切都在它该结束的时刻结束了。虽然考试凉了，但坑还是要接着填啊。为了方便和志同道合的朋友们交流心德，也是为了督促自己减少去安东星摸鱼的时间，我决定把项目公开出来。后排提醒，PCB线布的贼乱、代码bug更多，大佬轻喷。  
&emsp;目前项目取名为“进化”，计划使用STM32H750VBT6作为主控（性价比高），STM32F103C8T6作为协处理器（主控IO太少），3.5寸电容触摸屏（性价比高），固件基于FreeRTOS（文件夹还没建），界面基于LVGL，兼容主流航模遥控器高频头，自带通信模块仍是NRF24L01，但预留扩展接口，稍微遗憾的是由于H750的IO太少，音乐播放只能使用独立的MP3模块，但也降低了开发难度，算是一个取舍吧。  
&emsp;目前项目正在进行中，感兴趣的朋友们欢迎持续关注，可以关注我的bilibili账号“我的科技工作室”交流。 20210128
