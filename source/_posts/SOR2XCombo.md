---
title: SOR2XCombo readme document
date: 2023-10-26 14:11:00
tags: [OpenBor,Game]
---

# 怒之铁拳 Streets Of Rage 2X Combo


# 介绍
------------

怒之铁拳(Streets Of Rage)2X(以下简称SOR2X)是Kratus基于OpenBor引擎开发的横版卷轴过关游戏.
SOR2XCombo是我基于SOR2X2.3.1基础上开发的MOD.

因为SOR2X原项目所有可操作人物, 招式硬直比较大, 大部分特殊技没有合理的硬直取消, 加上空连和崩地的限制都很难进行长连段的连击.
为了增强游戏的爽快性, 我调整了几乎所有招式的性能, 使每个人物更好实现长连段的连击, 并且更加容易连携三星超必杀. 当然了, 可使用角色的增强, 对比之下原版的Boss就显得弱了. 很多其它SOR2X的MOD往往选择大幅加强主角的能力,但是各个Boss是没有变强的. 所以在打敌人的时候,无论小兵还是Boss都跟木头人一样,这样的敌人是没有灵魂的. 因此我也同样极大的增强了Boss的能力, 比如所有Boss现在都能够使用闪避, 防御, 空中受身, 弹反, 更强的连段攻击, 部分Boss加入了更多的招式, 等等...

**SOR2X**项目是一个免费游戏, 同样**SOR2XCombo**也是一个免费游戏. 作为作者, 我过去从来没有, 以后也永远不会通过这个MOD向任何玩家收费. 我MOD中使用的所有素材,包括图片,音频等(我写的代码除外)都是从互联网上搜集的. 它们的版权从来没有属于我. 我个人最看不上的就是使用别人未经授权的素材卖钱的行为.

我本人允许玩家对**SOR2XCombo**进行修改,前提是你不会拿我做的MOD去卖钱. 如果任何人拿去卖钱, 我保留我基于**SOR2X**项目所做修改(不包括网上素材部分)部分的追诉权力.

# 反馈

- 如果你也喜欢**SOR2XCombo**, 请加入QQ群  **657798865** , 我最新的Build都会发布在群里
- 如果你发现了关于**SOR2XCombo**的BUG, 请把 **Logs/OpenBorLog.txt**保存好, 或于群里留言, 或者去B站给我留言 [iintothewind](https://space.bilibili.com/29372518) 并发给我, 我会修复的.




# 特点
-------------

- 基础属性系统, 包括Skill, Power, Speed, Jump, Energy, 会影响角色的基础性能. Power对应攻击力,Speed对应移动速度,Jump对应跳跃高度, Energy对应能量恢复速度, Skill对应弹反后无敌的时间和弹反的能量恢复量.
- 弹反技能更容易使用,并且弹反成功以后,会进入短暂时间无敌,并且回复能量
- 连击狂热(Rush Heat)技能,连击数超过9以后会进入无敌状态,只要保持连击不断就一直是无敌状态
- 一线生机(Last Chance)技能,当处于空血状态并且防御槽全满时,遭受到下一次致命攻击时会恢复少量生命值
- 空连控制(Juggle System),可以控制敌人能够被空连的连击数上限,默认所有敌人都可以无限空连,当Juggle值被清空,则无法空连
- 崩地控制(OTG System),可以控制连击中敌人被崩地的次数,默认所有敌人都可以被无限次崩地,当OTG被清空,则无法攻击躺在地面的人
- 加入一代关卡, 并且可以在游戏开始的岔路口选择一代路线
- 每个小关卡都会随机刷出Boss,所以其实Boss的出现频率是非常高的
- 所有Boss的攻击招式都变强了,速度变快了,而且都会连招,部分Boss会无限连
- 战斗节奏加快了非常非常多,疯狂难度有类似忍者龙剑传超忍难度的体验

# 战斗逻辑
---------------

- **SOR2XCombo**的整体难度确实比原版难了很多,很多人觉得太难了,其实是对**SOR2XCombo**系统不够了解.
- **谨慎而适当的使用普通攻击**. 由于所有敌人的血量成倍的增加了,导致普通攻击的收益并不大. 我能理解很多人玩原版的习惯, 就是对Boss狂按普通攻击比如转身拳什么的,因为原版Boss会吃这一套. 但是在SOR2XCombo里面行不通: SOR2XCombo里面Boss的移动和攻击速度以及反应都非常快. 当你无脑的对着Boss连续按普通攻击时, 会非常容易被Boss弹反, 然后就会被Boss打一套连招扣大量生命值. 那么普通攻击就没用了吗? 不是的, 普通攻击不消耗能量值,当Boss被连段带入空中时,他们是没办法使用弹反的,这时候可以放心用普通攻击,并且普通攻击第三下按住下会使最后一下击飞攻击变为投技,把敌人抓住,然后使用投技,当你用投技击飞敌人到空中,又可以使用普通攻击,如此理论上可以无限连下去.

- **多使用弹反**. 弹反被设计成了一个回报非常大的技能. 我观察到很多玩原版的人是从来不用弹反这个技能的,因为原版的弹反需要看准时机按两个键,确实非常非常的难用,而且还消耗能量值.如此可说原版的弹反确实是个非常鸡肋的技能. 但是,弹反在SOR2XCombo里面却是一个比不可少的技能:
	* 你缺蓝了,用弹反,弹反能大量回蓝.
    * 你被敌人围攻了,用弹反,弹反能进入短暂无敌时间.
    * 你想狠扁Boss,用弹反,弹反后Boss会被浮空所以弹反技能往往就是连段的初始技能.

- **熟练使用能进入无敌状态的技能可以使战斗变的简单**. 我在系统中设计了非常多的手段能使操作角色进入无敌状态,熟练掌握这些技能,难度其实是很低的:
	* 闪避中会进入无敌状态
	* 弹反后会进入无敌状态
    * 连击数超过**9**会进入无敌状态
    * 部分角色使用投技会进入无敌状态,或者投技中翻过敌人头顶进入无敌状态
- **多使用冲刺投技和空中投技**. 几乎所有可操作人物比如Max,Blaze,Sammy等等角色,**前前Energy**是冲刺投技的,这样击飞的敌人冲过去就会被投技抓住,然后继续连段. 同样Max, Blaze, Shiva这些角色的空中特殊技也是投技, 对着空中的敌人一套连招, 最后还可以出投技把敌人砸向地面, 控制的好你的连击就是无限的.

- **弹墙攻击**. 某些角色比如Adam和Sammy的空中特殊技, 二代Shiva和Bison的超必杀是强力击飞技能, 会把浮空的敌人打到墙壁或者屏幕边上, 然后反弹回来, 利用这个特性带入连招, 可以造成大量长而华丽的连段.

- **连段中利用特殊技取消连三星超必杀**. 所有可操作角色都有一个以上的三星超必杀. 原版的超必杀是**下前Energy**, SOR2XCombo中可以在所有的特殊技动作中通过按**下加Special**或者**上加Special**来取消特殊技直接连超必杀, 比原版的出招方式要容易多了.

# 系统介绍
---------------

## 如何开启作弊菜单

Openbor引擎为所有OpenBor游戏提供了统一的作弊功能,他们的开启方法是一样的,进入游戏后,选择:
** Options -> System Options -> Cheats -> On **
这时候退回上一个菜单界面, 就会在System Options选项下面看到Cheats的选项已经显示了:
- Infinite Lives -> On 无限命
- Infinite Credits -> On 无限币
- Infinite Heath -> On 无限生命值
- Multihit Glitch -> On 多人连击同一目标, **打疯狂难度建议关掉**, 因为开着的话面对敌人前后夹击时你会死的很惨.

注意有些游戏是默认禁止了作弊功能,这种游戏里这些选项是没办法打开的,但SOR2XCombo是允许使用作弊功能的.

## 按键设置 (PC端)
** Options -> Control Options -> Setup Player 1 ... ** 进入玩家1的按键设置

- **Up**   				上
- **Down** 				下
- **Left**  			左
- **Right** 			右
- **Attack** 			攻击
- **Energy**			能量,通常也是带入空连的按键
- **Dodge/Block**		闪避/防御, 按住这个按键是防御, 先按方向键, 再按这个键是朝按住的方向闪避
- **Extra**		        额外按键, 默认是普通击飞攻击按键, 直接按这个键就出普通连段的最后一击, 如果按住下再按这个键就是朝后攻击,对攻击身后的敌人有用,不过更多的时候是当把浮空的Boss打到版边以后,按下再按这个键出向后攻击会把Boss从版本拉回,然后换个方向继续连击. 如果持有武器,按下加这个键就是扔出武器.
- **Jump**				跳跃,跳入空中后按方向键上或者下,或者不按方向键,再攻击,会出三种不同的跳攻击.这些跳攻击是没有硬直的,理论上你有多快的手速切换这三种跳攻击就能打浮空的敌人多少下,这是浮空连击的技巧之一,对原版也适用.
- **Special**			特殊技,在地面时按这个键出击飞特殊技,这个是保险技,出保险技的时间角色会进入无敌状态,是被攻击之后的保命技能.按前加这个按键,是攻击特殊技,可作为连段使用.在空中按这个键也会使用空中特殊技,部分人物的空中特殊技是投技,可以把浮空的敌人抓下来.
- **Start**				开始键,游戏中也是暂停键
- **Select**			选择键,游戏中按这个键是打开Extra Menu,可以选择CPU同伴等.

## 按键设置 (手机端)
** Extra menu -> controls -> Touch Layout ** 可以选择虚拟按键的布局
左边是方向键就不多说了, 右边:

- **A**					Attack,红色,攻击键
- **J**					Jump,跳跃,,跳入空中后按方向键上或者下,或者不按方向键,再攻击,会出三种不同的跳攻击,这些跳攻击时没有硬直的,理论上你有多快的手速切换这三种跳攻击就能打浮空的敌人多少下,这是浮空连击的技巧之一,对原版也适用.
- **S**					Special,特殊技,在地面时按这个键出击飞特殊技,这个是保险技,出保险技的时间角色会进入无敌状态,是被攻击之后的保命技能.按前加这个按键,是攻击特殊技,可作为连段使用.在空中按这个键也会使用空中特殊技,部分人物的空中特殊技是投技,可以把浮空的敌人抓下来.
- **A2**				Energy,能量,通常也是带入空连的按键
- **A3**				Dodge/Block,闪避/防御, 按住这个按键是防御, 先按方向键, 再按这个键是朝按住的方向闪避
- **A4**				Extra Button,额外按键, 默认是普通击飞攻击按键, 直接按这个键就出普通连段的最后一击, 如果按住下再按这个键就是朝后攻击,对攻击身后的敌人有用,不过更多的时候是当把浮空的Boss打到版边以后,按下再按这个键出向后攻击会把Boss从版本拉回,然后换个方向继续连击. 如果持有武器,按下加这个键就是扔出武器.
- **Select**			屏幕下方正中间ESC和Start两个按键中间靠上一点的位置,选择键,游戏中按这个键是打开Extra Menu,可以选择CPU同伴等.

## Extra Menu 额外菜单介绍
进入游戏后选择Extra Menu进入次菜单
### Extra Menu -> Game Play 游戏性选项

- Difficult 难度选择,默认是Normal难度,可选Normal,Hard,Mania. **Mania**是疯狂难度,敌人的攻击欲望是最强的.
- Enemy Life Rage 敌人血量控制,控制每次新游戏时敌人的血量上限,可以选择25%到200%
- Lives 每个币有几条命
- Last Chance Recover 一线生机(Last Chance)技能的生命回复量,当处于空血状态并且防御槽全满时,遭受到下一次致命攻击时会恢复少量生命值,可以控制回复生命的百分比
- Counter Attack Reward 弹反回报比率,设置弹返成功后恢复的能量值和无敌时间的百分比,默认100%,可以完全关闭则弹返成功不恢复多余能量并且完全没有无敌时间, 也可以设置为200%则弹返成功后恢复2倍能量和2倍无敌时间.
- Rush Heat 连击狂热(Rush Heat)技能,连击数超过9以后会进入无敌状态,只要保持连击不断就一直是无敌状态, 默认开启
- Juggle System 设置敌人进入空连后的空连值. 每个敌人都有空连值, 敌人被空连之后这个值会一直减少, 当空连值为0时,敌人便无法被继续空连了.默认为100
- OTG System 设置敌人崩地的次数. 每个敌人在连招中都有崩地上限, 当敌人被连招击中时触地这个值都会减少1,当OTG为0时,触地的敌人都没办法被继续打起来了,默认为10
- Enemy Rush Limit 敌人的连击数上限,限制敌人的最高连击数,当Boss的连击数超过限制,Boss会被迫使用闪避或者防御,打断Boss的连击,默认为无上限(Unlimited). 如果你不能接受被Boss无限连,就给Boss设置连击上限吧.
- Super Armor 超级护甲, 某些可控角色(比如Max,Sammy,Zan)或者Boss(Abadede,Bear)专属技能,当防御槽满时,可以完美抵御敌人的一次攻击
- Special Moves Cost 特殊技消耗类型, 默认特殊技消耗能量值, 可以选择消耗生命值, 或者类似与三代OK Bar那样随时间恢复, 默认请保持SOR2X Energy Only不要变, 这个涉及游戏机制, 选项变了游戏机制就全变了.
- Full Energy 每次进入新场景,新地图时保持能量全满,默认开启
- Walls 默认All Types, 敌人被击飞到墙壁会被反弹
- Screen Edge 默认All Types, 敌人被击飞到版边会被反弹
- Item Drop 物品掉落, Mix随机掉落所有物品,Food Only只掉落食物,Money Only只掉落钱,Weapon Only只掉落武器,或者其它组合
- Smarter Enemy 更加聪明的AI, 开启敌人的读按键技能,当玩家一直按下防御的时候,Boss不会无脑攻击,而是尝试快速靠近出投技
- Get Food 敌人主动去抢食物

### Extra Menu -> Controls 控制选项

- Block Type 默认Hold,按住防御键以后会一直防御
- Run Type 默认SOR2X,可以选择斜方向(Z轴)跑
- Dodge Type 默认SOR2X,按住方向键按防御键是朝按住的方向闪避, 可以换成SOR3,这样的话**上上,下下**也可以在Z轴闪避
- Jump Type 默认SOR2X,跳后不能控制方向, 如果换成SOR3则控制可以用方向键控制在空中的方向
- Extra Button 默认Charge Attack,按**Extra**按键出普通击飞攻击按键, 直接按这个键就出普通连段的最后一击. 如果改成Back Attack, 则默认出向后攻击, 但是不建议.
- Command List 出招表,一些简单的出招介绍,当然如果你如果能看懂英文也不需要我说明啥了.
- Touch Layout 手机上可以设置按键的布局

### Extra Menu -> Feature 特性控制

- Level Select 通关一次后,把这个选项设置为on, 则每次进入新游戏后可以选关

### Extra Menu -> Partners 伙伴控制

- Fighting Mode 战斗模式, Balanced平衡型,Aggressive进攻型,Defensive防御型
- Aggression 进攻欲望,9颗星为仇恨值最高
- Get Food 默认50%, 伙伴50%血量以下时会主动吃食物
- Follow Caller 默认**Automatic** 主动跟随玩家, 不要变
- Spawn/Kill 进入游戏后,按**Select**键,可选择呼出的伙伴,然后按下**A**召唤同伴. 召唤的同伴会跟你共享剩余生命数,当剩余生命数为1时则无法继续召唤. 如果你不想使用同伴喜欢,可以在这个选项再按A则让场上的同伴消失.

## 游戏内界面

进入游戏后,上方显示每个人物的图像和其它信息,
每个可操作角色都会显示生命槽,能量槽,和防御槽.
- **生命槽** 每个人物图像下方最大的那个血条
- **防御槽** 生命槽最外层的方框,在防御时遭受攻击,防御槽会减少. 大部分人物防御值最大为20,每秒回复5.
- **能量槽** 每个人物生命槽下方的星星,能量槽满值为5颗星星,超必杀会消耗三颗星,保险招消耗一颗星. 大部分人物能量值最大为120. 能量值靠普通攻击敌人,被敌人攻击,弹反等来恢复.

如果攻击敌人, 则在这些下方显示敌人的名字和血量,然后在敌人血量槽下方, 显示

- **K.O** 杀死敌人数量
- **DMG** 给敌人当前连击造成的伤害
- **HIT** 连击数
- **JUG** 如果Juggle System设置了空连上限,则显示当前敌人剩余的可连击值
- **OTG** 如果OTG System设置了崩地上限,则显示当前敌人剩余的可崩地次数

# 可操作角色
-----------------

## 角色通用技能
| 按键  |招式   |派生   |
|---|---|---|---|---|
|**Block**键按住不放|**防御**,敌人攻击会消耗防御槽,防御槽空会被破防|防御中敌人攻击瞬间按前或者后是弹反|
|弹反|防御时, 敌人攻击瞬间按**前**|敌人会出现硬直,自动反击敌人,并进入短暂无敌时间和回复大量能量. 进入无敌时间和能量回复跟每个人的技巧属性相关,技巧等级越高无敌时间和能量回复量越高. |
|按住方向按**Block**|向所按方向**闪避**,会短暂进入无敌状态|如果Doge Type为SOR3则按上上,下下可Z轴闪避. 无硬直,不消耗能量或者防御,可以一直闪避|
|被击飞到空中时按**上加跳**|**空中受身**,非常有用的保命技能,消耗四分之一防御槽. |因为SOR2XCombo敌人攻击节奏非常快,如果你被打浮空不使用空中受身的话,很容易被敌人无限浮空连,所以这个可能是频繁用到的技能. |
|倒地后按**上A**|起身攻击|快速起身并反击敌人.很多Boss非常擅长用这一招,所以靠近倒地后的Boss需要注意防御及时弹反.但有些Boss的起身攻击是投技,这时候防御正好被Boss抓投,所以还是需要快速反应.|
|**Extra** |普通攻击最后一段,强力击飞敌人. 可以配合按住**方向键前或者后**再按Extra调整身位 |可接多种特殊技,或者三星必杀  |
|**下Extra**| 攻击背后的敌人 |对在版边的浮空敌人出这一招则可以将版边的敌人拉回屏幕中间继续连招, 硬直短, 可在出招完后接其它招|
|连段中**连续按Energy**|**斜小跳**接跳攻击|在连段中使用,可以跳起继续连击浮空后的敌人,由于硬直短且不消耗能量,所以长连段里非常有用|
|被前后夹击按**Special**|**保险特殊技**,非常有用的保命技能,同时攻击前后敌人,消耗一颗星. |如果被前后夹击,或者处于被攻击状态,你会频繁用到这个技能. |
|连段中**下加Special**|消耗三星的必杀技|也可**下前Energy**直接出|
|空中**A**|不带入方向的跳攻击|可接**快速连按Energy**接斜小跳后跳攻击切换,也可接**Special**空中特殊技作为空连收尾招|
|空中**前A**|空中前攻击,一般是飞腿,可以将敌人踹飞的技能|可接**快速连按Energy**接斜小跳后跳攻击切换,也可接**Special**空中特殊技作为空连收尾招|
|空中**下A**|空中下攻击,如果击中敌人通常会快速抓住敌人下落,某些人物可以自动施展投技|击中敌人则快速抓住敌人到地面|
|空中**上A**|空中上攻击,可以将浮空的敌人往斜上方打|可接**快速连按Energy**接斜小跳后跳攻击切换,也可接**Special**空中特殊技作为空连收尾招|
|反擒|敌人投技抓你的瞬间按**A**|某些角色会施展投技反击,某些角色则会后退一段距离|
|持武器**下Extra**|扔出武器,部分武器可投掷多次|部分情况出现武器无限扔的情况属于脚本执行bug|
|被动技能|一线生机(Last Chance)技能,清空防御槽|当处于空血状态并且防御槽全满时,遭受到致命攻击时会恢复少量生命值. |
|被动技能|连击狂热(Rush Heat)技能|连击数超过9以后会进入无敌状态,只要保持连击不断就一直是无敌状态|
|被动技能|超级护甲(Super Armor)技能,消耗二分之一防御槽|部分角色(Max,Sammy,Zan等)专属技能,当防御槽全满时,等自动抵挡一次攻击.|


## Axel

Axel攻击力, 速度, 技巧, 能力回复速度都属于中等, 是一个很平衡的角色.
Axel的普通攻击速度很快, 侧重直接攻击的打击系, 特殊技是快速出拳的连打, 空中地面都可以用, 所以非常好上手, 缺点是特殊技接三星超必杀时会把敌人拉回地面, 这样有些敌人会在连招的间隙就瞬移闪避掉了, 造成连段失败.

| 按键  |招式   |派生   |
|---|---|---|---|---|
|A连按  |普通攻击1123连打, 第四下出二连侧踹   | 如果第三下按住方向键下, 则第四下会改为投技抓住敌人  |
|**Extra**|直接出二连侧踹,也可按住前后方向调整身位 |**前前A** 上勾拳, **前前Energy** 升龙拳, **下加Special**可以出三星必杀技陀螺升龙拳, 按上加Special可以出三星必杀幻影拳, **快速连按Energy**斜小跳空中跳攻击空连  |
|**前前A**|上勾拳, 最后一击将会使敌人浮空, 不消耗能量 |**Extra** 二连侧踹, **下加Special**可以出三星必杀技陀螺升龙拳, **上加Special**可以出三星必杀幻影拳, 快速连按Energy可以进行空中跳攻击空连 |
|**前前Energy**|升龙拳, 转身2周后接升龙, 会将敌人打浮空, 同时会附带火焰伤害, 消耗少量能量 |在地面的时候, 连段同前前A, 在空中的时候, 可以按**Special**消耗少量能量接空中连打, 也可以**快速连按Energy**斜小跳,进行跳攻击快速切换 |
|**Special**|360火焰拳, 保险招, 出招时是无敌状态, 被击中的敌人会被击飞|硬直短, 可在出招完后接其它招   |
|**前Special**|地面连打, 然后出升龙拳|**前前A** 上勾拳, **前前Energy** 升龙拳, 地面连打的时候如果能量剩余三星以上, **下加Special**可以出三星必杀技陀螺升龙拳, **上加Special**可以出三星必杀幻影拳,**快速连按Energy**斜小跳,可以进行空中跳攻击空连|
|**连段中下加Special**|三星必杀技陀螺升龙拳,强力必杀技,攻击中会封印敌人的特殊技,打满整个连段附带火焰伤害 |也可**下前Energy**直接出, 不过建议用在特殊技后取消连超必杀. 在连段中,假如敌人会瞬移闪避,被上一招击中时敌人处于地面状态,按**下加Special**连这招三星必杀时,疯狂难度的敌人有概率会瞬移闪避,导致超必杀打空. 破解办法就是连超必杀尽量晚一点,等上一招发完,把Boss击飞到空中时恰好被释放超必杀,恰好能打中Boss,那Boss就会被从空中拉下来|
|**连段中上加Special**|三星必杀技幻影狮子拳,强力大范围必杀技,覆盖半个屏幕的大范围攻击|无直接出招方式只能靠特殊技取消连段派生. 这招在连段中不存在Boss会瞬移闪避掉的问题,但在版边或者有障碍物时因为距离原因会存在判定失败问题.|
|按住**前**抓住敌人A|膝撞,可以连撞两下,第三下将会将敌人击飞出去|硬直短, 可在出招完后接其它招  |
|抓住敌人按**A**|头锤,将敌人直接击飞|硬直短, 可在出招完后接其它招  |
|抓住敌人按后**A**|后仰摔,将敌人摔向身后|硬直短, 可在出招完后接其它招  |
|抓住敌人按跳|翻身跳,按住敌人跳到敌人身后,可进入短暂无敌状态|可继续用投技|
|翻身跳以后按**A**|翻身跳投,抓住敌人砸向地面|硬直短, 可在出招完后接其它招  |
|空中**Special**|空中连打|建议用在**快速连按Energy**斜小跳,空中跳攻击空连之后,作为空中收招|
|弹反|防御时, 敌人攻击瞬间按前, 出升龙拳,火属性攻击敌人 |在空中的时候, 可以按**Special**消耗少量能量接空中连打, 也可以**快速按Energy**进行跳攻击快速切换|
|持匕首A|匕首普通攻击,不再击飞敌人,可持续攻击|被敌人攻击则武器掉落,掉落地上的武器30秒后会被系统回收|
|持苦无A|苦无普通攻击,不再击飞敌人,可持续攻击|被敌人攻击则武器掉落,掉落地上的武器30秒后会被系统回收|
|持钢管A|击飞敌人|被敌人攻击则武器掉落,掉落地上的武器45秒钟会被系统回收|
|持刀A|击飞敌人|被敌人攻击则武器掉落,掉落地上的武器60秒钟会被系统回收|
|持刀前前A|幻影剑,大范围攻击,不消耗能量|无取消连招,最后一击敌人会被击飞|
|持刀A接下A|剑气攻击,消耗三颗星|剑气不可防御|

## Blaze

Blaze同样也是比较平衡的角色, 攻击力比Axel稍弱, 但是速度比Axel要稍快, 所以两个人平分秋色.
Blaze偏技巧型角色, 普通攻击同样很快, 打击能力没有Axel强, 不过她同时拥有地面冲刺投技和空中投技, 所以连段其实更加丰富多样.

| 按键  |招式   |派生   |
|---|---|---|---|---|
|**A连按**|普通攻击1123连打, 第四下出高角度正踹|如果第三下按住方向键下, 则第四下会改为投技抓住敌人 |
|**Extra**|直接出普攻第四下出高角度正踹,也可按住前后方向调整身位|**下加Special**可以出三星必杀技千鸟,**快速连按Energy**斜小跳,可以进行空中跳攻击空连|
|**前前A**|360空翻接手刀|空中时, **快速连按Energy**斜小跳,可以进行空中跳攻击空连, 按**Special**则使用空中投技将敌人抓住砸向地面|
|**前前Energy**|冲刺抓投,冲刺过程非无敌,抓投破防,对空有效|经常用在一个连段结束,对待击飞的敌人使用,可以将在空中或者地上的敌人重新抓起继续连招|
|**Special**|后空翻脚刀,保险招, 出招时是无敌状态, 被击中的敌人会被击飞|**前前A** 360空翻接手刀, **前前Energy** 冲刺抓投, **Extra** 直接出普攻第四下出高角度正踹, 按**下加Special**可以出千鸟,**快速连按Energy**斜小跳,可以进行空中跳攻击空连|
|**前Special**|波动拳,地面连打,最后一击敌人会被击飞地面,消耗少量能量|**前前A** 360空翻接手刀, **前前Energy** 冲刺抓投, **Extra** 直接出普攻第四下出高角度正踹,如果能量剩余三星以上,按**下加Special**可以出千鸟,**快速连按Energy**斜小跳,可以进行空中跳攻击空连|
|连段中**下加Special**|三星必杀千鸟,强力必杀技,攻击中会封印敌人的特殊技,打满整个连段附带雷电伤害|也可**下前Energy**直接出, 不过建议用在特殊技后取消连超必杀. 在连段中,假如敌人会瞬移闪避,被上一招击中时敌人处于地面状态,按**下加Special**连这招三星必杀时,疯狂难度的敌人有概率会瞬移闪避,导致超必杀打空. 破解办法就是连超必杀尽量晚一点,等上一招发完,比如出**前Special**波动拳时,需要打到最后一击,把Boss击飞到空中时恰好被释放超必杀,恰好能打中Boss,那Boss就会被从空中拉下来|
|按住**前**抓住敌人连续按A|膝撞,可以连打两下,第三下会扇敌人一巴掌|保持按**方向前**不变,因为距离敌人身位很近,打完第三下又会将敌人抓住,可以无限连下去. 不过这一招非无敌状态,实战中会被敌人打断,而且Boss是打不完三下就会挣脱的,所以无限连只对普通敌人并且无干扰时有用  |
|抓住敌人按**A**|按倒敌人,使其崩到地面反弹|**前或者后Extra**普攻第四下出高角度正踹,将崩地的敌人从地面踢起来, **前前A** 360空翻接手刀, **前前Energy** 冲刺抓投  |
|抓住敌人按**后A**|后仰摔,将敌人摔向身后|硬直短, 可在出招完后接其它招  |
|抓住敌人按**跳**|翻身跳,按住敌人跳到敌人身后,可进入短暂无敌状态|可继续用投技|
|翻身跳以后按**A**|翻身跳投,抓住敌人砸向地面|硬直短, 可在出招完后接其它招  |
|空中**下A**|空中下攻击,如果击中敌人会快速抓住将敌人后仰摔|后仰摔可继续空连|
|空中**Special**|空中投技,按倒敌人,使其崩到地面反弹|建议用在**快速连按Energy**斜小跳,空中跳攻击空连之后,作为空中收招使用|
|弹反|防御时, 敌人攻击瞬间按前, 出滑铲,对空有效 | **前或者后Extra** 普攻第四下出高角度正踹,将崩地的敌人从地面踢起来, **前前A** 360空翻接手刀, **前前Energy** 冲刺抓投|
|持匕首A|匕首普通攻击,不再击飞敌人,可持续攻击|被敌人攻击则武器掉落,掉落地上的武器30秒后会被系统回收|
|持匕首前前A|匕首升龙,出招过程无敌|匕首升龙时没跳到空中以前,都可以接**下Special**匕首乱舞|
|持匕首前**Special**|匕首乱舞,出招过程无敌|可以接**下Special**匕首乱舞必杀|
|前两招中**接下Special**|匕首乱舞必杀,消耗能量很少|无取消连招|
|持苦无A|苦无普通攻击,不再击飞敌人,可持续攻击|被敌人攻击则武器掉落,掉落地上的武器30秒后会被系统回收|
|持钢管A|击飞敌人|被敌人攻击则武器掉落,掉落地上的武器45秒钟会被系统回收|
|持刀A|击飞敌人|被敌人攻击则武器掉落,掉落地上的武器60秒钟会被系统回收|
|持刀前前A|幻影剑,大范围攻击,不消耗能量|无取消连招,最后一击敌人会被击飞|

## Max

- Max是一个擅长投技的力量型角色, 移动速度和攻击速度都比较慢, 但是力量等级是5, 目前主角里面力量等级最高的.
- Max的生命值很高, 并且拥有超级护甲(Super Armor)被动技能, 所以防御很不错.
- Max拥有丰富的投技, 虽然没办法打出长连击但是凭借空中投技和地面投机的连携, 也能打出非常华丽的连击.
- Max抓住敌人和使用空中投技以后会进入短时间无敌状态.
- Max拥有三种三星必杀技,连段中**下加Special**出横臂冲击,抓住敌人A投技出头槌时接**上Special**原地大坐, 接**下Special**拱桥背摔.
- Max的连招非常依赖**Extra键**双拳下砸,连招中**快速连按Energy**斜小跳接空连,空中靠近浮空敌人按**Special**空中投技这几招来实现以投技为主的连招.
- Max的能量恢复比较慢. 如果没有能量的情况下, 可以按住**下加A连按**方式实现普通攻击接投技的连招攒齐三颗星以后,接**上加Special**出三星必杀原地大坐, 或者接**下加Special**出三星必杀拱桥背摔.

| 按键  |招式   |派生   |
|---|---|---|---|---|
|**A连按**|普通攻击1123连打, 第四下出抱拳下砸|如果第三下按住方向键下, 则第四下会改为投技抓住敌人 |
|**Extra** |直接出普攻第四下出抱拳下砸,也可按住前后方向调整身位|**下加Special**可以出三星必杀,**快速连按Energy**斜小跳,可以进行空中跳攻击空连|
|**前前A**|滑铲,可以快速接近敌人|**快速连按Energy**斜小跳毁容踢,可以进行空中跳攻击空连, **Special**旋转拳,**前Special**肩撞冲刺|
|**前前Energy**|冲刺抓投,冲刺过程非无敌,抓投破防,对空有效|经常用在一个连段结束,对待击飞的敌人使用|
|**Special**|旋转拳,保险招, 出招时是无敌状态, 被击中的敌人会被击飞|**前前A**滑铲, **前前Energy**冲刺抓投, **Extra**直接出普攻第四下出抱拳下砸, **前加Special**肩撞冲刺,**快速连按Energy**斜小跳,可以进行空中跳攻击空连|
|**前Special**|肩撞冲刺,多次攻击敌人,最后一击敌人会被击飞地面,消耗少量能量|**前前Energy** 冲刺抓投, **Extra** 直接出普攻第四下出双拳下砸,**Special斜小跳空中抓投**,**快速连按Energy**斜小跳,可以进行空中跳攻击空连|
|连段中**下加Special**|三星必杀横臂冲击,强力必杀技,将敌人击飞,到版边回弹|也可**下前Energy**直接出, 不过建议用在特殊技后取消连超必杀.|
|按住**前**抓住敌人**连续按A**|膝撞,可以连打两下,第三下出头槌|前两下膝撞可以接**跳**,抓住敌人到空中|
|抓住敌人按**A**|锁颈接头槌|可按住下加普通攻击三联后按下接投技接这招,可以轻松无限连,头槌时接**上Special**三星必杀原地大坐, 头槌时接**下Special**三星必杀拱桥背摔|
|上一招出头槌时**上Special**|三星必杀原地大坐|强力摔投,摔投后敌人浮空可继续连招|
|上一招出头槌时**下Special**|三星必杀拱桥背摔|强力摔投,摔投后敌人浮空可继续连招|
|抓住敌人按**后A**|后仰摔,将敌人摔向身后|硬直短, 可在出招完后接其它招  |
|抓住敌人按**跳**|抓住敌人到空中|**speical**空中投技坐头摔,**前spcial**将敌人摔向地面|
|空中**下A**|空中下攻击,如果击中敌人通常会快速抓住敌人下落|可继续使用投技|
|空中靠近浮空敌人按**Special**|空中投技坐头摔|抓住浮空的敌人坐向地面,并附带短时间无敌. 建议用在**快速连按Energy**斜小跳,空中跳攻击空连之后,作为空中收招使用|
|弹反|防御时, 敌人攻击瞬间按前, 出旋转拳,对空有效 |**前前A**滑铲, **前前Energy**冲刺抓投, **Extra**直接出普攻第四下出抱拳下砸, **前加Special**肩撞冲刺,**快速连按Energy**斜小跳,可以进行空中跳攻击空连|
|持匕首**A**|匕首普通攻击,不再击飞敌人,可持续攻击|被敌人攻击则武器掉落,掉落地上的武器30秒后会被系统回收|
|持苦无**A**|苦无普通攻击,不再击飞敌人,可持续攻击|被敌人攻击则武器掉落,掉落地上的武器30秒后会被系统回收|
|持钢管**A**|击飞敌人|被敌人攻击则武器掉落,掉落地上的武器45秒钟会被系统回收|
|持钢管**A**中接**下Special**|三星必杀钢管强力攻击|敌人会被强力砸倒|
|持刀**A**|击飞敌人|被敌人攻击则武器掉落,掉落地上的武器60秒钟会被系统回收|


## Sammy

- 轮滑小子Sammy是主角团队中个子最矮并且生命值最低的, 但他是身手敏捷的速度型角色. 他的速度,技巧,能量点数都是4点, 意味着他从来不缺能量, 大招可以随便放, 不过攻击力跟Blaze一样都是2点.
- 虽然Sammy生命值低, 但是Sammy同样拥有超级护甲(Super Armor)被动技能, 但由于生命值比较低, 超级护甲在空血时并不会提供太多保护.
- Sammy抓住敌人和翻身跳以后会进入短时间无敌状态. Sammy的翻身跳后骑敌人脖子施展王八拳连打敌人头部时也会进入无敌状态,不会被其他人打到.
- Sammy也是原版唯一一个可以在空中释放三星必杀技的角色.
- Sammy的武器特殊技最多. 几乎所有武器Sammy都可以**前前A**出空中旋风斩并且旋风斩中可以接**下Special**三星必杀超级旋风斩, 持钢管时Sammy地面前Special还可以出钢管插地大回旋.
- Sammy空手时的连招也很丰富, 空连时按**Special**出后空翻可以将敌人踢飞到版边然后弹回,实现丰富的空连.


| 按键  |招式   |派生   |
|---|---|---|---|---|
|**A连按**  |普通攻击1123连打, 第四下出后空翻踢|如果第三下按住方向键下, 则第四下会改为投技抓住敌人 |
|**Extra**   |直接出普攻第四下后空翻踢,也可按住前后方向调整身位|**下加Special**可以出三星必杀空中电钻,**快速连按Energy**斜小跳可以进行空中跳攻击空连|
|**前前A**|前空翻接头槌,可以快速接近敌人|空中时,**快速连按Energy**斜小跳飞腿可以进行空中跳攻击空连, **Special**后空翻强力踢击将敌人击飞到版边回弹, **Extra**直接出普攻第四下后空翻踢|
|**前前Energy**|冲刺抓投,冲刺过程非无敌,抓投破防,对空有效|经常用在一个连段结束,对待击飞的敌人使用|
|**Special**|地面扫腿,保险招, 出招时是无敌状态, 被击中的敌人会被击飞|**快速连按Energy**斜小跳,可以进行空中跳攻击空连|
|**前Special**|王八拳连打接后空翻踢飞,可按**方向前或后**调整身位|非常实用的技能,通常用在连招中可以快速增加连击数.可接**快速连按Energy**斜小跳飞腿可以进行空中跳攻击空连, **Special**后空翻强力踢击将敌人击飞到版边回弹, **Extra**直接出普攻第四下后空翻踢,地面或者空中时都可以接**下Special**三星必杀空中电钻|
|连段中**下加Special**|三星必杀空中电钻,强力必杀技,空中地面都可以出|也可**下前Energy**直接出, 不建议地面直接出这招,因为前摇过长,敌人会在命中之前躲开. 建议在空中时用特殊技后取消连超必杀,或者抓住敌人时按**A**后空翻踢飞敌人之前, 按**下Special**, 因为此时敌人无法躲避.|
|按住**前**抓住敌人**连续按A**|头槌,可以连打两下,第三下出肘击|前两下头槌可以接**跳**,翻过敌人头顶|
|抓住敌人按**A**|后空翻踢飞|敌人没有被击飞之前按**下加Special**三星必杀地面电钻|
|抓住敌人按**后A**|后空翻踢飞|硬直短, 可在出招完后接其它招|
|抓住敌人按**跳**|翻身跳,按住敌人跳到敌人身后,可进入短暂无敌状态|可继续用投技|
|翻身跳过程中按**A**|翻身摔投|将敌人向前摔出|
|翻身跳后按**A**|骑敌人脖子上,王八拳连打头部,可进入短暂无敌状态|灵魂投技,整个出招过程也是无敌的|
|空中**下A**|空中下攻击,如果击中敌人通常会快速抓住敌人下落|可继续使用投技|
|空中按**Special**|后空翻强力踢击将敌人击飞到版边回弹|敌人回弹后可继续空连,部分敌人能够使用空中受身则无法回弹|
|弹反|防御时, 敌人攻击瞬间按前, 出后空翻踢接月牙波,对空有效 |**前前A**前空翻头槌, **前前Energy**冲刺抓投, **Extra**直接出普攻第四下后空翻踢, **前加Special**王八拳连打,**快速连按Energy**斜小跳,可以进行空中跳攻击空连|
|持匕首**A**|匕首普通攻击,不再击飞敌人,可持续攻击|被敌人攻击则武器掉落,掉落地上的武器30秒后会被系统回收|
|持匕首**前前A**|匕首旋风斩|旋风斩空中连击,可接**下Special**三星必杀超级旋风斩|
|持苦无**A**|苦无普通攻击,不再击飞敌人,可持续攻击|被敌人攻击则武器掉落,掉落地上的武器30秒后会被系统回收|
|持苦无**前前A**|苦无冲刺|苦无冲刺攻击,可接**下Special**三星必杀超级旋风斩|
|持钢管**A**|击飞敌人|被敌人攻击则武器掉落,掉落地上的武器45秒钟会被系统回收|
|持钢管**前前A**|钢管旋风斩|旋风斩空中连击,可接**下Special**三星必杀超级旋风斩|
|持钢管**前Special**|钢管插地大回旋|最后一击敌人浮空|
|持刀**A**|击飞敌人|被敌人攻击则武器掉落,掉落地上的武器60秒钟会被系统回收|
|持刀**前前A**|武士刀旋风斩|旋风斩空中连击,可接**下Special**三星必杀超级旋风斩|
|持武器旋风斩中接**下Special**|三星必杀超级旋风斩|强力必杀,最后一击敌人浮空|


## Adam

- Adam是SOR2X原版中二周目解锁的隐藏角色之一,他的属性值中能量和跳跃只有一点,攻击力和Blaze,Sammy持平,唯有技巧属性比较高为4点.从属性分配可以看出他的能量恢复比较多依靠弹反攻击, 因为他的生命值比Sammy要高不少, 所以可以看作是更加容易上手的技巧性角色.
- Adam的标志性技能是**前前Energy**发出的月牙波和带有弹墙效果的空中特殊技能**空中Special**超人拳, 他的连招也多依赖这两招.
- Adam拥有两种三星必杀技,连段中**下加Special**可以出三星必杀乱舞连击, **上加Special**可以出三连重击.

| 按键  |招式   |派生   |
|---|---|---|---|---|
|**A连按**|普通攻击1123连打, 第四下出侧踢|如果第三下按住方向键下, 则第四下会改为投技抓住敌人 |
|**Extra**|直接出普攻第四下侧踢,也可按住前后方向调整身位|**下加Special**可以出三星必杀乱舞连击, **上加Special**可以出三连重击, **快速连按Energy**斜小跳可以进行空中跳攻击空连|
|**前前A**|上勾拳,最后一击敌人浮空|**快速连按Energy**斜小跳飞腿可以进行空中跳攻击空连, **Extra**直接出普攻第四下侧踢|
|**前前Energy**|**标志性技能**,上勾拳后接月牙波|常用在距离超出近身攻击范围的连击中,集中使敌人浮空,然后快速接近继续连击|
|**Special**|360勾拳,保险招, 出招时是无敌状态, 被击中的敌人会被击飞|**快速连按Energy**斜小跳,可以进行空中跳攻击空连|
|**前Special**|前冲直拳,弹墙技能,强力击飞敌人到版边然后回弹|非常实用的技能,对待不能空中受身的敌人非常有效,当地人从版本反弹回来时可继续连招.**下加Special**可以出三星必杀乱舞连击, **上加Special**可以出三连重击, **快速连按Energy**斜小跳可以进行空中跳攻击空连|
|连段中**下加Special**|三星必杀乱舞连击,强力必杀技,空中地面都可以出|也可**下前Energy**直接出, 最后一击敌人浮空,可继续连招|
|连段中**上加Special**|三星必杀三连重击,强力必杀技,空中地面都可以出|也可**下前Energy**直接出, 最后一击敌人浮空,可继续连招|
|按住**前**抓住敌人**连续按A**|膝撞,可以连打两下,第三下出肘击|前两下头槌可以接**跳**,翻过敌人头顶|
|抓住敌人按**A**|抓住敌人按头崩地|硬直短, 可在出招完后接其它招|
|抓住敌人按**后A**|过肩摔|硬直短, 可在出招完后接其它招|
|抓住敌人按**跳**|翻身跳,按住敌人跳到敌人身后,可进入短暂无敌状态|可继续用投技|
|翻身跳后按**A**|后仰摔|向后摔投,硬直短, 可在出招完后接其它招|
|空中**下A**|空中下攻击,如果击中敌人通常会快速抓住敌人下落,施展后仰摔投|摔投后可继续连击|
|空中按**Special**|**标志性技能**,超人拳,强力冲拳将敌人击飞到版边回弹|这招经常用于空连的收尾技能,将敌人打到版边回弹后可继续空连,部分敌人能够使用空中受身则无法回弹|
|弹反|防御时, 敌人攻击瞬间按前, 出侧踢,对空有效 |**前前A**上勾拳, **前前Energy**月牙波, **Extra**直接出普攻第四下侧踢, **前加Special**前冲直拳,**快速连按Energy**斜小跳,可以进行空中跳攻击空连|
|持匕首**A**|匕首普通攻击,不再击飞敌人,可持续攻击|被敌人攻击则武器掉落,掉落地上的武器30秒后会被系统回收|
|持苦无**A**|苦无普通攻击,不再击飞敌人,可持续攻击|被敌人攻击则武器掉落,掉落地上的武器30秒后会被系统回收|
|持钢管**A**|击飞敌人|被敌人攻击则武器掉落,掉落地上的武器45秒钟会被系统回收|
|持刀**A**|击飞敌人|被敌人攻击则武器掉落,掉落地上的武器60秒钟会被系统回收|
|持刀**前前A**|武士刀冲刺|多段冲刺攻击,最后一击敌人浮空,可接**下Special**武士刀三星必杀|
|上一招中接**下Special**|三星必杀武士刀冲刺|强力必杀,最后一击敌人浮空|

## Zan

- Zan是SOR2X原版中二周目解锁的隐藏角色之一,一个老头外形的机器人,擅长使用电属性攻击.他的基础属性值中能量和跳跃也是只有一点,攻击力比较高为4点.从属性分配可以看出他是一个偏重力量的技巧型角色.
- Zan的标志性技能是持武器后三星必杀,按**下前Special**释放追踪能量球,这个技能是所有角色中伤害时间最长伤害最大的超必杀,当然也是最无聊的. 因为被能量球沾上的敌人会一直被攻击直到能量球消失, 中间你什么都不需要做.
- Zan三种放电特殊技分别是**Special**全身放电, **前Special**电爪, 空中**Special**空中电爪, 都可以用在连击里面.

| 按键  |招式   |派生   |
|---|---|---|---|---|
|**A连按**|普通攻击112连打, 第三下出直拳|如果第二下下按住方向键下, 则第三下会改为投技抓住敌人 |
|**Extra**|直接出普攻第三下直拳,也可按住前后方向调整身位|**下加Special**可以出三星必杀电球连放, **快速连按Energy**斜小跳可以进行空中跳攻击空连|
|**前前A**|肩撞冲击,最后一击敌人浮空|**快速连按Energy**斜小跳可以进行空中跳攻击空连, **Extra**直接出普攻第三下直拳|
|**前前Energy**|冲刺抓投,冲刺过程非无敌,抓投破防,对空有效|经常用在一个连段结束,对待击飞的敌人使用,可以将在空中或者地上的敌人重新抓起继续连招|
|**Special**|全身放电,保险招, 出招时是无敌状态, 被击中的敌人会被击飞|**快速连按Energy**斜小跳,可以进行空中跳攻击空连|
|**前Special**|电爪,最后一击击飞敌人|**下加Special**可以出三星必杀电球连放, **快速连按Energy**斜小跳可以进行空中跳攻击空连|
|连段中**下加Special**|三星必杀电球连放,强力必杀技|也可**下前Energy**直接出, 最后一击敌人浮空,可继续连招. 建议用在**前Special**电爪或者**Extra**直拳之后,因为攻击距离够远而且会定住敌人,正好接这招|
|按住**前**抓住敌人**连续按A**|爪击,可以连打两下,第三下出重拳|保持按**方向前**不变,因为距离敌人身位很近,打完第三下又会将敌人抓住,可以无限连下去. 不过这一招非无敌状态,实战中会被敌人打断,而且Boss是打不完三下就会挣脱的,所以无限连只对普通敌人并且无干扰时有用 |
|抓住敌人按**A**|抓住敌人下砸崩地|硬直短, 可在出招完后接其它招|
|抓住敌人按**后A**|向后摔投|硬直短, 可在出招完后接其它招|
|抓住敌人按**跳**|翻身跳,按住敌人跳到敌人身后,可进入短暂无敌状态|可继续用投技|
|翻身跳后按**A**|向后摔投|向后摔投,硬直短, 可在出招完后接其它招|
|空中**下A**|空中下攻击,如果击中敌人通常会快速抓住敌人下落|可继续使用投技|
|空中按**Special**|**标志性技能**,空中电爪|这招经常用于空连的收尾技能,被电攻击的敌人空中无法受身,可继续连击|
|弹反|防御时, 敌人攻击瞬间按前, 出肩撞冲击,对空有效 |**前前A**肩撞冲击, **前前Energy**冲刺抓投, **Extra**直接出普攻第三下直拳, **前Special**电爪,**快速连按Energy**斜小跳,可以进行空中跳攻击空连|
|持武器**前前A**|释放能量球|伤害比较小切不能改变方向|
|持武器**下前Special**|释放追踪能量球|伤害巨大但是无聊的超必杀,被能量球击中的敌人会一直挨打,一个打不死建议放两个|


## SOR2 Shiva

- 二代Shiva是SOR2XCombo添加到主角团队中的隐藏角色, 各属性值比较平均都是3点, 唯独速度为4点. 想玩好二代Shiva你需要非常快的手速输入, 因为二代Shiva的强项是所以角色中空连最强的, 通过合理利用波动拳补能完全可以在空连中连续释放多次超必杀.
- 二代Shiva的标志性技能为能强力击飞敌人弹墙的**前前A**波动拳, 命中后能恢复大量能量
- 二代Shiva的空中特殊技空中**前Special**龙尾踢, 必杀技空中连段中**下Special**必杀龙尾踢, 配合弹墙技能**前前A**波动拳可以组成非常华丽的弹墙空连.
- 不过二代Shiva的连招因为招式前揺比较大, 为了增强命中, 他非常依赖**前前Energy**冲刺抓投. 面对浮空后的敌人二代Shiva都需要用冲刺抓投快速接近抓住敌人, 然后才能施展各种特殊技, 这样敌人才不会轻易躲开.

| 按键  |招式   |派生   |
|---|---|---|---|---|
|**A连按**|普通攻击112连打, 第三下出高挑腿|如果第二下下按住方向键下, 则第三下会改为投技抓住敌人 |
|**Extra**|直接出普攻第三下高挑腿,也可按住前后方向调整身位|**前前A**波动拳,**前加Special**龙尾踢,**下加Special**可以出三星必杀龙尾踢,**上加Special**三星必杀无影掌,**快速连按Energy**斜小跳可以进行空中跳攻击空连|
|**下Extra**|翻身挑腿,火属性击飞敌人,击中敌人后空中**翻身转向**|**翻身以前可以连招**,在地面可连**前前A**波动拳,地面空中都可连**前加Special**龙尾踢,**下加Special**可以出三星必杀龙尾踢,**上加Special**三星必杀无影掌,**快速连按Energy**斜小跳可以进行空中跳攻击空连,**Extra**直接出普攻第三下高挑腿|
|**前前A**|**标志性技能**波动拳,弹墙技能,强力击飞敌人到版边回弹,**命中敌人后回复大量能量**.|**快速连按Energy**斜小跳可以进行空中跳攻击空连, **Extra**直接出普攻第三下高挑腿,**上加Special**三星必杀无影掌|
|**前前Energy**|冲刺抓投,冲刺过程非无敌,抓投破防,对空有效|经常用在一个连段结束,对待击飞的敌人使用,可以将在空中或者地上的敌人重新抓起继续连招|
|**Special**|返身踢,保险招, 出招时是无敌状态, 被击中的敌人会被击飞|**快速连按Energy**斜小跳,可以进行空中跳攻击空连,**前前A**波动拳,**Extra**直接出普攻第三下高挑腿|
|**前Special**|龙尾踢,击飞敌人,最后一段带火属性攻击|**上加Special**空中抓投,**下加Special**三星必杀龙尾踢, **快速连按Energy**斜小跳可以进行空中跳攻击空连|
|连段中**上加Special**|三星必杀无影掌,攻击范围非常大,**命中敌人后回复大量能量**.|最后一击敌人浮空,可以继续空连|
|连段中**下加Special**|三星必杀龙尾踢,强力必杀技,弹墙技能,击中后敌人会撞向版边回弹,可继续连招|也可**下前Energy**直接出,不过建议用在**前Special**龙尾踢或者**下Extra**翻身挑腿将敌人击浮空之后. 因为此时身位合适,这招命中率最高|
|按住**前**抓住敌人**连续按A**|勾拳连击,这招会维持短暂无敌状态|保持按**方向前**不变,因为距离敌人身位很近,打完第三下又会将敌人抓住,可以无限连下去. |
|抓住敌人按**A**|直接出普攻第三下高挑腿|硬直短, 可在出招完后接其它招|
|抓住敌人按**后A**|抓住敌人向后砸向地面崩地|建议用在**前前Energy**冲刺抓投之后,可以将敌人很方便的打浮空|
|抓住敌人按**跳**|翻身跳,按住敌人跳到敌人身后,可进入短暂无敌状态|可继续用投技|
|翻身跳后按**A**|抓住敌人砸向地面崩地|硬直短, 可在出招完后接其它招|
|空中**下A**|空中下攻击,如果击中敌人通常会快速抓住敌人砸向地面崩地|崩地后可继续连击|
|空中按**Special**|空中抓投,抓住敌人砸向地面|这招经常用于空连的收尾技能,但因为二代Shiva空连技能有更强大的龙尾踢,所以只是作为补充技能.|
|弹反|防御时, 敌人攻击瞬间按前, 返身踢 |**前前A**波动拳, **前前Energy**冲刺抓投,**上加Special**三星必杀无影掌,**Extra**直接出普攻第三下高挑腿,**快速连按Energy**斜小跳,可以进行空中跳攻击空连|


## SOR3 Shiva

- 三代Shiva作为SOR2XCombo添加到主角团队中的隐藏角色, 是目前所有可控角色中最强大的一个.
- 三代Shiva的标志性技能**前前A**无影掌, 不需要能量就能直接释放, 攻击范围非常大, 并且命中后大量补充能量.
- 三代Shiva拥有连击数非常多的特殊技**前Special**龙爪连击, 和连击数更多的三星必杀连段中**下Special**龙爪连击.
- 以上三招还可以无缝连接, 所以很容易就无限连了.

| 按键  |招式   |派生   |
|---|---|---|---|---|
|**A连按**|普通攻击112连打, 第三下出高挑腿|如果第二下下按住方向键下, 则第三下会改为投技抓住敌人 |
|**Extra**|直接出普攻第三下高挑腿,也可按住前后方向调整身位|**前前A**无影掌,**前加Special**龙爪连击,**下加Special**可以出三星必杀龙爪连击, **快速连按Energy**斜小跳可以进行空中跳攻击空连|
|**下Extra**|翻身挑腿,火属性击飞敌人,击中敌人后空中**翻身转向**|**翻身以前可以连招**,在地面可连**前前A**无影掌,地面空中都可连**前加Special**龙爪连击,**下加Special**可以出三星必杀龙爪连击, **快速连按Energy**斜小跳可以进行空中跳攻击空连,**Extra**直接出普攻第三下高挑腿|
|**前前A**|**标志性技能**无影掌,不需要能量就能直接释放, 攻击范围非常大,**命中敌人后回复大量能量**.|最后一击敌人浮空,可以继续空连|
|**前前Energy**|冲刺抓投,冲刺过程非无敌,抓投破防,对空有效|经常用在一个连段结束,对待击飞的敌人使用,可以将在空中或者地上的敌人重新抓起继续连招|
|**Special**|返身踢,保险招, 出招时是无敌状态, 被击中的敌人会被击飞|**快速连按Energy**斜小跳,可以进行空中跳攻击空连,**前前A**无影掌,**Extra**直接出普攻第三下高挑腿|
|**前Special**|龙爪连击,最后一段带火属性攻击击飞敌人.这招能量消耗少连击数却非常多,但缺点是攻击距离比较短,前揺较长.|这一招面对会瞬移闪避的Boss是打不中他们的,因此为了增加命中率,建议先用**前前Energy**冲刺抓投抓住敌人,然后使用这一招.被投技抓住的敌人是没办法瞬移闪避的,所以可以百分百命中. 这招可以连**下加Special**三星必杀龙爪连击大量扣血, **快速连按Energy**斜小跳可以进行空中跳攻击空连,**Extra**直接出普攻第三下高挑腿|
|连段中**下加Special**|三星必杀龙爪连击,强力必杀技|也可**下前Energy**直接出,这一招同样有攻击距离太短的缺点,直接释放打不到人,建议用在**前Special**龙爪连击之后,或者先用**前前Energy**冲刺抓投抓住敌人,然后使用这一招|
|按住**前**抓住敌人**连续按A**|勾拳连击,这招会维持短暂无敌状态|保持按**方向前**不变,因为距离敌人身位很近,打完第三下又会将敌人抓住,可以无限连下去. |
|抓住敌人按**A**|直接出普攻第三下高挑腿|硬直短, 可在出招完后接其它招|
|抓住敌人按**后A**|抓住敌人向后砸向地面崩地|建议用在**前前Energy**冲刺抓投之后,可以将敌人很方便的打浮空|
|抓住敌人按**跳**|翻身跳,按住敌人跳到敌人身后,可进入短暂无敌状态|可继续用投技|
|翻身跳后按**A**|抓住敌人砸向地面崩地|硬直短, 可在出招完后接其它招|
|空中**下A**|空中下攻击,如果击中敌人通常会快速抓住敌人砸向地面崩地|崩地后可继续连击|
|空中按**Special**|空中抓投,抓住敌人砸向地面|这招经常用于空连的收尾技能.|
|弹反|防御时, 敌人攻击瞬间按前, 波动拳, 弹墙技能 |**前前A**无影掌, **前前Energy**冲刺抓投, **Extra**直接出普攻第三下高挑腿,**快速连按Energy**斜小跳,可以进行空中跳攻击空连|

## SOR2 Electra

- 二代鞭女是SOR2XCombo添加到主角团队中的原创角色,她的速度和技巧都为4,是一个速度非常快的技巧型角色.
- 二代鞭女的招牌技能是电鞭发射, 发射出去的电鞭会将敌人定住, 并且三星必杀将会快速接近敌人然后释放大范围鞭打攻击.
- 二代鞭女的冲刺抓投速度非常快, 并且拥有回血的18X投技.

| 按键  |招式   |派生   |
|---|---|---|---|---|
|**A连按**|普通攻击112连打, 第三下出高挑腿|如果第二下下按住方向键下, 则第三下会改为投技抓住敌人 |
|**Extra**|直接出普攻第三下高挑腿,也可按住前后方向调整身位|**前前A**升龙鞭,**前加Special**电鞭发射,**下加Special**可以出三星必杀电鞭连打, **快速连按Energy**斜小跳可以进行空中跳攻击空连|
|**下Extra**|后摆腿|攻击版边浮空敌人,将敌人拉回屏幕中央|
|**前前A**|升龙鞭|**前加Special**电鞭发射,**下加Special**可以出三星必杀电鞭连打, **快速连按Energy**斜小跳可以进行空中跳攻击空连|
|**前前Energy**|冲刺抓投,冲刺过程非无敌,抓投破防,对空有效|经常用在一个连段结束,对待击飞的敌人使用,可以将在空中或者地上的敌人重新抓起继续连招|
|**Special**|电鞭360连打,保险招, 出招时是无敌状态, 被击中的敌人会被击飞|**快速连按Energy**斜小跳,可以进行空中跳攻击空连,**前前A**升龙鞭,**Extra**直接出普攻第三下高挑腿|
|**前Special**|电鞭发射,将敌人定住,最后一击敌人浮空|这一招的攻击距离很远,对待浮空的敌人很有效. 这招可以连**下加Special**三星必杀电鞭连打大量扣血, **前前A**升龙鞭,**Extra**直接出普攻第三下高挑腿|
|连段中**下加Special**|三星必杀电鞭连打,先用电鞭发射定住敌人,然后快速接近电鞭连打,强力必杀技|也可**下前Energy**直接出,建议用在**前Special**电鞭发射之后|
|按住**前**抓住敌人**连续按A**|膝撞连击,非无敌状态|保持按**方向前**不变,因为距离敌人身位很近,打完又会将敌人抓住,可以将普通敌人无限连下去. |
|抓住敌人按**A**|鞭打连击,非无敌状态|硬直短, 可在出招完后接其它招|
|抓住敌人按**后A**|18X投技,完事后恢复少量生命|硬直比较大,无法继续连其它招|
|空中**下A**|空中下攻击,如果击中敌人通常会快速抓住敌人下落|可继续使用投技|
|空中按**Special**|空中升龙鞭|这招经常用于空连的收尾技能.|
|弹反|防御时, 敌人攻击瞬间按前, 升龙鞭, 弹墙技能 |**前前A**升龙鞭, **前前Energy**冲刺抓投, **Extra**直接出普攻第三下高挑腿,**快速连按Energy**斜小跳,可以进行空中跳攻击空连|


## SF2 Bison

- 街霸2拳王Bison是SOR2XCombo添加到主角团队中的原创角色, 他的力量最高为5点, 跳跃和能量都为1点, 是一个偏重力量的角色.
- 拳王的特点就是能量恢复是非常慢的, 但是他普通攻击比较重, 侧重于普通攻击和特殊技的组合连招.

| 按键  |招式   |派生   |
|---|---|---|---|---|
|**A连按**|普通攻击1234连打, 第四下出上勾拳|如果第三下下按住方向键下, 则第四下会改为投技抓住敌人 |
|**Extra**|直接出普攻第四下上勾拳,也可按住前后方向调整身位|**前前A**垫布直拳,**前加Special**组合拳连打,**下加Special**可以出三星必杀乱舞连击, **快速连按Energy**斜小跳可以进行空中跳攻击空连|
|**下Extra**|下摆拳|攻击版边浮空敌人,将敌人拉回屏幕中央|
|**前前A**|垫布直拳|**前加Special**组合拳连打,**下加Special**可以出三星必杀乱舞连击, **快速连按Energy**斜小跳可以进行空中跳攻击空连|
|**前前Energy**|冲刺抓投,冲刺过程非无敌,抓投破防,对空有效|经常用在一个连段结束,对待击飞的敌人使用,可以将在空中或者地上的敌人重新抓起继续连招|
|**Special**|直拳360连打,保险招, 出招时是无敌状态, 被击中的敌人会被击飞|**快速连按Energy**斜小跳,可以进行空中跳攻击空连,**前前A**垫布直拳,**Extra**直接出普攻第四下上勾拳|
|**前Special**|组合拳连打,将敌人定住,最后一击敌人浮空|这招可以连**下加Special**三星必杀乱舞连击大量扣血, **上加Special**腾空头锤,**前前A**垫布直拳,**Extra**直接出普攻第四下上勾拳|
|**上Special**|腾空头锤,对空特殊技|**空中Special**头锤,**Extra**直接出普攻第四下上勾拳|
|连段中**下加Special**|三星必杀乱舞连击,强力必杀技,**弹墙技能**,最后一击敌人强力击飞到版边回弹|也可**下前Energy**直接出|
|按住**前**抓住敌人**连续按A**|下勾拳击腹,非无敌状态|保持按**方向前**不变,因为距离敌人身位很近,打完又会将敌人抓住,可以将普通敌人无限连下去. |
|抓住敌人按**跳**|抓住敌人跳到空中|可接**A**,出空中头槌,效果同空中**Special**|
|抓住敌人按**A**|头锤,无敌状态|硬直短, 可在出招完后接其它招|
|抓住敌人按**后A**|转身头锤,无敌状态|硬直短, 可在出招完后接其它招|
|空中**下A**|空中下攻击,如果击中敌人通常会快速抓住敌人下落|可继续使用投技|
|空中按**Special**|空中头锤,投技|这招经常用于空连的收尾技能.|
|弹反|防御时, 敌人攻击瞬间按前, 垫布直拳|**前前A**垫布直拳, **前前Energy**冲刺抓投, **Extra**直接出普攻第四下上勾拳,**快速连按Energy**斜小跳,可以进行空中跳攻击空连|



# 部分Boss角色
-----------------------

## Abadede

- 角斗士阿巴德, 力量型Boss, 三星必杀不可防御, 弹反不可防御, 擅长飞扑
- 角斗士阿巴德善于利用冲刺上勾拳和冲刺抓投进行二择攻击, 让玩家在防御与攻击直接出现判断失败, 从而造成巨大伤害.
- 他的三星必杀因为速度很快且不可防御, 很难躲避.
- 不要尝试距离角斗士阿巴德太近, 因为他的近身特殊技狂战怒吼为多段攻击, 被他技狂战怒吼击浮空会大量扣血,被打浮空后就面临接下来他的连续技飞扑投技或者上勾拳.
- 他还拥有飞扑技能, 飞扑同样不可防御, 注意闪避或者直接攻击, 按防御则会被他摔出去.

## Ash

- 变性人船长Ash, 是一个非常擅长投技的力量型Boss
- 他的大招投技判定很强, 不要在他用大招过来抓你的时候跟他用特殊技拼招, 你会很容易被他抓住.
- 他的投技有一招可以XX玩家, 然后回血.
- 等他靠近, 他有时候会尝试使用普通攻击, 这时候你可以弹反他, 或者击飞他, 然后用连招打他.
- 或者距离比较远, 等他嘲笑你的时候, 快速接近用连招打他.
- 反擒技能强的角色打他会很有优势, 等他过来用投机抓你的瞬间按**A**出反擒技能, 某些角色比如Max,二代Shiva等此时就会用投技反击.

## Rocky Bear

- 拳击手洛基熊, 力量型Boss, 招牌技能连续升龙拳, 和升龙拳接三星必杀超级升龙拳.
- 拳击手洛基熊同样会使用前勾拳和冲刺抓投进行二择攻击, 一旦命中玩家, 则会选择使用连续升龙拳, 如果三星以上则尝试取消升龙接三星必杀技.
- 拳击手洛基熊近身会出弹墙技能,短距离下勾拳, 被击中会打到版边然后回弹.

## Barbon

- 调酒师巴本, 擅长踢击的Boss. 他的弹反非常精准, 被他弹反击中会被扫腿打飞.
- 调酒师巴本靠近玩家后会频繁使用冲刺抓投, 可以躲避, 或者趁他过来时用击飞技能打飞他.
- 不要在他能量多时靠近他, 他的三星必杀连环踢腿威力很大.

## Harkiri

- 重甲武士Harakiri, 擅长拔刀术和爆破追踪手里剑的武士.
- 重甲武士Harakiri拥有两种类型, 进攻型Harakiri会主动靠近并攻击玩家, 防守型Harikiri则会跟玩家拉开距离, 但玩家进入他的近身范围他才会尝试攻击,或者更多用弹返打击玩家.
- 重甲武士Harakiri在距离玩家较远的时候会投出多枚追踪手里剑, 尽量攻击打掉或者持续闪避躲掉. 如果手里剑靠近时一直防御, 则会被手里剑从背后击中引起爆炸, 面临大量伤害. 此时Harikiri则会靠近玩家, 施展拔刀术接三星必杀幻影斩, 一套就被带走了.
- 玩家如果被Harakiri普通拔刀术击中, 玩家会被打浮空, 而Harakiri会快速瞬移到玩家身后发动第二次拔刀术攻击, 如果防御不及时, 接下来就是一连串攻击接三星必杀幻影斩, 轻易就被带走了.
- 因为他会瞬移闪避, 玩家的普通攻击是打不到他的. 最好的打法就是玩家要持续利用闪避的无敌帧靠近Harakiri, 等他出近身拔刀术, 然后弹反攻击打浮空以后再连招打他.
- 玩家被Harakiri打浮空, 要及时使用空中受身, 落地时注意看Harakiri的站位, 选择争取方向防御, 准备随时弹反攻击.
- 对付防守型的Harakiri千万不要一直按防御键. 你防御他就会马上瞬移到你身后用投技抓你. 最好用闪避移动到他跟前, 然后等他出招, 弹反他然后用连招打他.

## Yamato

- 红铠武士Yamato, 是游戏里面技能最华丽的Boss. 因为他非常擅长瞬移, 速度非常快, 因此是弱点最少的Boss.
- 红铠武士Yamato拥有两种类型, 偏重剑术攻击的类型Musashi, 偏重忍术攻击的类型Yamato.
- 偏重剑术攻击的类型Musashi比较擅长隐身瞬移到玩家身后出拔刀术接三星必杀幻影斩. 偏重忍术攻击的类型Yamato则比较擅长使用影分身冲刺接三星必杀幻影斩.
- 红铠武士Yamato同样会瞬移, 并且移动速度非常快. 玩家所有的正面攻击是根本打不到他的, 任何攻击还没靠近他. 他就会瞬移躲开, 并且此时玩家有硬直, 他会出现在玩家背后, 利用玩家出招后的硬直打一套连击. 所以最好不要正面打他, 你跟不上他的速度.
- 对付红铠武士Yamato的最好策略是, 首先多弹反他的攻击积攒能量, 等他出现在玩家身后出拔刀术时, 出360保险招, 他靠近时会被玩家的保险招打浮空, 然后打一套连招对付他.
- 红铠武士Yamato离玩家中段距离是会尝试快速瞬移到玩家跟前冲刺抓投玩家, 被他抓住他会使用投技饭纲落. 他的投技速度很快, 而且会来回跑动多次, 注意他移动的残影, 及时闪避, 攻击和防御都会被他抓住.
- 红铠武士Yamato离玩家非常进的时候会翻滚腾空释放3枚手里剑, 如果你躲过他的三枚手里剑, 在他翻滚下落的过程中他会尝试从空中抓住你施展投技饭纲落.
- 对付剑术攻击型的Musashi千万不要一直按防御键. 你防御他就会马上瞬移到你身后对你用饭纲落. 最好等他对你用拔刀术的时候, 用保险招把他打下来, 然后用连招打他.

## Zamza

- 利爪忍者Zamza, 是一个移动速度非常快的Boss.
- 利爪忍者Zamza在你防御时会尝试用滑铲滑倒玩家, 然后用投技, 如果你中了投技, 在站立过程中, 他会继续用滑铲接投技, 如此你会一直被他投技连下去, 破掉这个循环你需要站立瞬间马上用保险招, 他会躲开.
- 利爪忍者Zamza有时也会从空中跳到玩家身边, 施展空中下落的投技, 如果你中了投技, 在你空中受身的过程中, 很可能会继续被他从空中抓住, 这个连续空中抓投比较难躲, 不过他没有足够能量不会重复很多次,
- 利爪忍者Zamza也会使用连续的升龙爪, 中了他的升龙爪要及时受身躲开.

## Bruce & Roo

- 持皮鞭的小丑驯兽师布鲁斯和袋鼠小路是一对一起出现的Boss. 小丑的皮鞭擅长远距离攻击, 而袋鼠速度快擅长近距离缠斗.
- 小丑的三星大招会释放炸弹陷阱, 如果玩家中了陷阱会被吊起到空中, 要及时受身躲开. 如果玩家没有中陷阱, 则过6秒钟后, 陷阱会触发大范围爆炸, 爆炸对敌人同样有效. 因此玩家可以利用这个特性, 在爆炸时, 通过闪避的无敌帧将敌人引到陷阱周围, 炸到敌人.
- 袋鼠Roo的大招是冲刺抓投, 速度快注意及时闪避. 它的弹反攻击是旋风腿, 多段攻击, 被他打到扣血也很多.

## Jet & Rocket

- 飞人Jet & Rocket, 是两个会飞行的敌人. Jet拥有三星必杀冲刺抓投, Rocket同样也会三星必杀冲刺抓投, 并且他还会三星必杀火焰喷射, 和特殊技浮游炸弹.
- 这两个Boss速度很快, 追着他们打不是很好的策略. 最好是站原地, 等他俯冲攻击, 让抓准这个时机用弹反攻击打他们.
- 用弹返打到他们以后将这两个Boss打浮空, 然后尽量用**Energy连按**的跳攻击空连打他们.

## Tracker

- 铁血战士Tracker是一个会隐身锁定玩家释放不可防御追踪离子炮的Boss.
- 铁血战士Tracker释放三星必杀时, 会隐身并尝试锁定玩家, 此时玩家最好一直利用闪避的无敌帧躲避, 等他锁定玩家一段时间, 会在玩家身后出现, 瞬间释放不可防御的追踪离子炮. 如果此时玩家没有闪避, 则会被不可防御的追踪离子炮击中, 大量扣血. 如果此时玩家一直闪避则处于无敌状态, 不可防御的追踪离子炮会靠近玩家但无法击中, 很快消失.
- 铁血战士Tracker的另一个特殊技是普通离子炮, 为可防御技能, 但是普通离子炮有可能从背后击中玩家, 不过伤害并不大.
- 被铁血战士Tracker的冲刺抓投抓住以后, 他会使用近身电击爪攻击玩家, 此时玩家处于麻痹状态, 无法用保险招反击, 然后他会尝试接升龙, 要及时受身闪避.
- 铁血战士Tracker空中跳攻击会变为空中抓投, 被他从空中抓住他也会用近身电击爪攻击玩家, 此时玩家处于麻痹状态, 无法用保险招反击, 最后一击玩家会被打浮空, 他经常会重复空中抓投, 然后玩家又一次中招, 如此直到他能量耗尽或者放弃空中抓投连招...

## Break

- Axel的复制人Break是一个危险的Boss, 他拥有Axel的所有技能, 并且随着血量减少, 他的移动速度和攻击速度会越来越快.
- 面对玩家, Break会尝试用冲刺快速靠近, 玩家会面临他冲刺上勾拳和冲刺抓投的二择, 如果选错, 他将会打玩家一套连招.
- 在能量足够的情况下, Break的每次投技和特殊技都有可能以狮子幻影拳收尾, 这一招攻击范围非常打, 速度很快, 因此非常难躲.
- 面对残血状态的Break, 他会进入移动速度和攻击速度超级快的疯狂状态, 尽量用连招结束他, 否则很容易被他反杀.

## 三代Shiva

- 作为Boss的三代Shiva同样是一个令玩家头疼的Boss, 因为被他任意一招击中都有可能被他打无限连.
- 他的跳攻击下压掌会从空中抓住玩家, 然后玩家就会中他的投技, 所以他空中的下压掌不要防御.
- 尽量与他拉开距离, 然后弹反他的攻击, 顺带尽可能用连招打他.

## RobotX

- 三代出场的量产型机器人, 手臂可以发射追踪火箭弹
- 他的追踪火箭弹需要一直闪避过一段时间会自动爆炸
- RobotX近身可施展全身放电, 一旦被他的三星必杀全身放电击中有可能会被秒

## Mr.X

- X先生,存在感不强的最终Boss, 手持机枪, 可以远程多方向射击, 三星大招也是追踪火箭弹
- 他的追踪火箭弹需要一直闪避过一段时间会自动爆炸
- Mr.X闪避玩家攻击时会扔出手榴弹,
- 玩家靠近他, 他会尝试冲刺抓投玩家, 并施展三拳一脚投技踢开玩家, 并投掷一枚手榴弹

## Monalisa Sisters

- 蒙娜丽莎姐妹组合, 擅长跳攻击和配合攻击的Boss, 她们的大招地面波速度很快但是可以防御
- 不要被姐妹俩前后夹击, 她们会同时出腿然后疯狂连击, 此时防御基本不起作用, 很快被连死
- 被她们的跳攻击击中后, 她们会施展空中投技, 离她们很近距离的情况下她们也会尝试冲刺抓投, 但是冲刺速度很慢, 由于距离很近也不是很好预测, 总之看到她们身发红光靠近就说明她们要抓投你了.
- 姐妹俩有时候会施展组合技攻击, 不过用的并不会很频繁


# Enemy 部分杂兵
-------------

## Galsia

- 加西亚, 身穿牛仔裤, 牛仔马甲的普通小兵, 有时候会捡匕首
- 被手持匕首的加西亚攻击会被攻击多次并迅速倒地
- 加西亚还会一招跳起肘击下砸, 不过用的机会并不多

## Donovan

- 唐纳文, 身穿牛仔裤, 赤裸上身的光头小兵, 有时候会持钢管出场
- 空手的唐纳文重击会出上勾拳, 手持钢管的唐纳文攻击也会比较狠
- 如果玩家离被击倒的唐纳文很近, 他会快速起身出上勾拳, 这招反击力量还是很大的

## Signal

- 信号, 留莫西干发型的干瘦小兵, 速度敏捷, 擅长滑铲
- 信号有时出场会扔酒瓶攻击, 酒瓶扔的又快又准, 非常烦人, 建议优先解决
- 如果玩家离被击倒的信号很近, 他会用滑铲快速接近玩家把玩家摔出去

## Garnet

- 加奈特, 留短发穿短裙的小太妹, 距离远会跳起攻击, 距离近则会扇耳光
- 能量够的话, 加奈特会尝试跳起扑倒玩家, 然后主动求XX, 被她XX到玩家会扣血, 她则会加血


## Jack

- 小混混杰克, 二代路线里面第一关骑摩托车出场的飞刀手, 我个人最喜欢的一个杂兵
- 空手状态时, 杰克会掏出匕首, 然后远距离投飞刀攻击玩家
- 当近身靠近玩家时, 杰克会尝试持刀快速捅玩家, 如果玩家防御, 杰克则会尝试快速抓投破掉玩家的防御, 然后捅玩家三刀
- 无论杰克是否持到, 他近身都会弹反玩家的攻击
- 玩家被杰克打倒后, 杰克会得意的嘲笑倒在地上的玩家

## Electra

- 人气颇高的三代鞭女, 身穿露肩紧身衣和过膝长筒靴, 左手残疾但改成了一条电鞭
- 三代鞭女一般不会主动近身攻击, 当玩家接近, 如果能量够她会释放电鞭攻击, 否则使用普通鞭打, 然后尝试投技, 有时候会施展快速鞭打, 有时候则会主动求XX, 被她XX到玩家会扣血, 她则会加血
- 被玩家击倒她会鸭子坐起身装可怜, 此时玩家无法攻击

## Bigben & Bongo

- 会吐火的大胖子大笨 & 邦, 有时候他们会吐火攻击玩家, 有时候他们会施展肉弹战车
- 面对防御中的玩家, 有时候这俩大胖子会施展投技抓住玩家, 扔出去
- 如果玩家离被击倒的胖子很近, 他们会快速起身用肉弹战车反击, 这时候不要犹豫马上出弹反给他们来个停车吧

## Hakuyo & Raven & Tiger

- 哈库, 留小辫子赤裸上身的泰拳肌肉男, 特色技能会单手发气功波
- 如果被击倒时, 他们会快速起身用飞腿反击.
- 哈库会弹反玩家攻击, 弹反招式为气功波, 中他的弹返后玩家会被击飞弹墙
- 瑞文, 穿背心短裤的泰拳男, 特色技能膝撞
- 泰拳男会对玩家用投技, 同时也能弹反玩家攻击
- 瑞文被玩家击倒, 会快速起身用膝撞反击

## Kusanagi

- 草薙, 速度快的忍者, 有时候会持苦无或者武士刀出场
- 当他们空手状态时, 他们会释放手里剑骚扰玩家, 如果离玩家很近他们也会尝试使用投技
- 他们手持苦无或者武士刀时, 会施展旋风斩, 伤害比较大
- 他们空手和吃武器时都可以弹反玩家的攻击
- 这些忍者们移动速度快并且会连续闪避玩家的攻击

## Bruce

- 持皮鞭小丑的布鲁斯, 大招是释放炸弹陷阱
- 如果玩家踩中炸弹陷阱, 则会被吊起, 可以受身安全落地, 如果玩家没有踩中陷阱, 则6秒后陷阱触发大范围爆炸, 波及范围内所有敌人包括玩家. 玩家可以依靠闪避的无敌帧, 引诱敌人聚集到陷阱周围被炸弹炸死, 这个是**快速清场的秘诀**.
- 布鲁斯倒地后会快速起身, 用膝撞攻击玩家

