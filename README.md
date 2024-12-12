# 《名字待定》
## 1.引言
  《名字待定》是一个fps游戏。玩家将在游戏中扮演一个于塔底苏醒并失去记忆的角色，在通往塔顶的途中不断死亡重生，逐渐发现自己的来历与这座塔的真相。玩家将在关卡中遇到各式武器与附魔卡（名字后面可以改）。每种武器都有其独特的定位与功能。附魔卡可以直接使用，也可以用来强化武器使武器获得特殊功能。游戏将围绕武器与附魔卡的搭配进行肉鸽闯关。
## 2.玩家基本要素

### 2.1 玩家键位
  wasd 移动
  shift 疾跑
  space 跳跃
  q 切换武器
  r 换弹
  e 捡起武器
  t 为武器附魔
  esc 暂停界面
  f 直接使用附魔卡
  mouse1 开火
  mouse2 瞄准/武器功能
  ctrl 下蹲/滑铲
  i 打开背包

  ### 2.2 玩家基本功能
血量与护甲值
2个武器栏
20个附魔卡槽
30个背包栏位
左上角显示buff与debuff
疾跑时按下蹲触发滑铲，滑铲有cd但不显示（类似于apex的滑铲机制）
疾跑时无法开枪，可使用附魔卡
ui界面如下
![alt text](无标题.png)
## 3.武器
### 3.1武器品质
武器品质有:白色、淡蓝色、蓝色、紫色、红色、金黄色
白色：武器的基础样式，拥有一个附魔位置，无额外属性，稀有度为随处可见
淡蓝色：白色的加强款，一个附魔位置与一个额外属性，稀有度比白色更高
蓝色：两个附魔位置与两个额外属性，稀有度加加
紫色:三附三额
红色：三附四额
金色：特殊武器
### 3.2武器种类
1.霰弹：伤害较高，射速较慢，有较大的距离伤害衰减与精准度衰减
2.狙击：伤害高，射速慢，伤害随距离增加而提升
（以下省略伤害与射速等数据部分，主要讨论机制）
3.步枪：无特殊机制
4.手枪：半自动，可双持
5.剑：装备时移速提升，移动能力（如滑铲）冷却减少，右键格挡获得伤害减免并略微减速
6.匕首:冲刺并造成伤害
### 3.3武器额外属性
白色属性：少量吸血（近战）、燃烧效果...
蓝色属性：吸血（近战）、击杀死亡爆炸、快速换弹...
紫色属性：减少伤害获得小范围子弹追踪、将印记数量的50%增加至伤害...
红色属性：击杀回复子弹、增强附魔卡效果...

## 4.附魔卡
|附魔卡名字|直接使用|附魔强化|
|:---:|:---:|:---:|
|爆炸|向前进行大范围高伤害攻击|获得40发爆炸子弹/永久提高近战武器伤害|
|虚无|使5秒内受到的所有伤害变为1|与接下来该远程武器击杀的10个敌人交换位置并获得2秒无敌时间/近战武器获得0.5秒无敌时间|
|狂宴|对小范围内的敌人造成一次当前武器伤害 自身回复造成伤害总额一半的血量|10s内回复该武器造成伤害的10%生命|
|种子|获得100层印记|该武器每击杀一个敌人获得一层印记|
|果实|获得[种子]，清除所有印记，造成一次与印记数量相同的爆炸伤害|升级已有的[种子]附魔，提升为击杀一个敌人获得三层印记|
|牺牲|立刻随机获得3个附魔卡|当此武器被丢弃时，获得6个附魔卡|
|傲慢|无法直接使用，占用5个附魔卡位|无法附魔强化，当持有[傲慢]时，造成的伤害变为2倍，受到的伤害变为3倍|
|...|

## 5.关卡
### 5.1关卡形式
游戏分为三个区域，每个区域有n个关卡（包含两个boss关卡）从当前区域的关卡图池中进行选择，以不同路径而非选关界面来切换关卡
![alt text](无标ss题.png)
### 5.2关卡机制
* 关卡分为普通与困难，关卡地图布局相同但刷怪不同，且可能带有debuff。
* 困难有更多的收益以及更具挑战性的关卡。
* 关卡被生成时，有n%的概率为困难。
* 关卡与关卡之间可能存在宝箱房与商店房，这两个房间均可以打开仓库
 
 ## 6.场外成长
