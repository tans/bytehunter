代码仓 https://github.com/tans/byte-hunter

## 《字节猎人》GRPG Description


![image](https://user-images.githubusercontent.com/543287/129016595-8b50461f-1b5a-4ae8-9125-5a4005d1851b.png)



《字节猎人》是一个聊天室的文字rpg游戏， 本项目为游戏设定和方案的讨论。

群成员通过【出战】迎击聊天室中出现的怪物，获得战力提升， 同时提升群战力。
群战力影响不同等级的怪物出现。

## Monster
聊天室中出现的怪物

![image](https://user-images.githubusercontent.com/543287/129131248-58c67ffa-6045-4e63-82fb-417d99f5c550.png)

`HP 击杀奖励 出现间隔`

## Group
聊天室

`战力值`

## Member
成员 世界唯一，可存在于不同群中

`战力值 击杀冷却周期 击杀次数 上次击杀`

# 输出算法


```
realack = (ack) ->
	if ack > 1000000
		return (ack - 1000000) / 30 + 130000
	else if ack > 100000
		return (ack - 100000) / 10 + 40000
	else if ack > 10000
		return (ack - 10000) / 3 + 10000
	else
		return ack
    
realack(ack) *  random(0.8~1.2)

```

## 技能系统（todo）
成员通过习得的关键字触发技能。技能分伤害类和辅助类。

## 副本系统（todo）
群聊可以主动刷副本提升成员战力

## 世界排行

群聊战力排行

个人战力排行



![image](https://user-images.githubusercontent.com/543287/129016673-235b3206-6856-4bfc-9a21-95e425564e09.png)




## 入群体验
<img src="https://user-images.githubusercontent.com/543287/128971592-a54e6096-50f0-46e6-be9a-4c3b89939845.png" width="220px" />

## 加机器人, 拉机器人入群即可玩，仅支持企业微信外部群， 最好新拉群操作。
<img src="https://user-images.githubusercontent.com/543287/128972133-8648d2a5-e461-4382-85b8-c4428d36d3f6.png"  width="220px" />


