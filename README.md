#宏命令

##基础命令

- 施放：施放一个或多个技能,可以加入一些条件判断,是最常用的命令
```
/cast 
```
- 顺序施放：依次施放数个技能
```
/castrandom
```
- 随机施放
```
/castsequence
```
- 取消变形
```
/cancelform
```
- 取消状态或增益
```
/cancelaura
```
- 开始攻击：一般写不写差别不大，施放技能会自动开始攻击的
```
/startattack
```
- 停止攻击：与startattack相反，用于防止破除控制等功能
```
/stopattack
```
- 指定目标
```
/target
```
- 指定敌对目标
```
/targetenemy
```
- 指定上一个目标
```
/targetlasttarget
```
- 装备武器
```
/equip
```
- 指定位置装备
```
/equipslot
```
- 召唤坐骑
```
/mount
```
- 解散坐骑
```
/dismount
```
- 宏描述
```
#showtooltip
```
- 当前目标
```
%t
```
- 焦点
```
/focus
1.没有焦点目标的时候将目标设置为焦点目标
2.有焦点目标的时候将焦点目标更改成当前目标
3.当前目标为空时清空焦点目标
```
- 清除焦点
```
/clearfocus
```
- 停止宏命令
```
/stopmacro
```
- 控制命令
```
/script
```
- 运行脚本
```
/run
```
- 延迟命令
```
/in
```
- 点击动作条
```
/click ExtraActionButton1
```

##语言表情命令
- 普通频道（白字）
```
/s 
```
- 大喊（红字）
```
/y 
```
- 小队频道
```
/p
```
- 团队频道
```
/ra
```
- 表情命令（橙字）
```
/e
```

##判断命令
```
help 目标友方
harm 目标敌方
exists 目标存在
noexists 目标不存在
dead 目标死亡
nodead 目标存活
combat 战斗状态
nocombat 非战斗状态
stealth 潜行状态
nostealth 非潜行状态
nomod 未按下功能键
swimming 游泳状态
noswimming 非游泳状态
flyable 可飞行状态
noflyable 不可飞行状态
indoors 室内状态
outdoors 室外状态
mouseover 鼠标指向目标
pet 目标宠物
player 目标玩家
mod:XXX 按下功能键 [alt/shift/ctrl/button1/button2/button3/...]
```

- 判定条件
```
[target=XXX]
```
- 重置条件
```
reset=XXX
```

##方法命令
- 目标上标记
```
SetRaidTarget("target", X) // X为1~8
1 星星
2 大饼
3 菱形
4 三角
5 月亮
6 方块
7 红叉
8 骷髅
```
- 购买物品
```
BuyMerchantItem(index [, quantity])
index // 物品序号
quantity // 物品数量
```