# Nixware功能说明

#### legitbot <a href="#user-content-1.1" id="user-content-1.1"></a>

<figure><img src="../../../.gitbook/assets/image (11) (2).png" alt=""><figcaption></figcaption></figure>

*   **Globals**

    Enable：开启合法bot，一般绿演使用\
    Attack team：开启友伤，开启后当敌人和队友在同一枪线上时依旧开火\
    Smoke check：烟雾检查\
    Flash check：闪光检查\
    Scope check：开镜检查\
    Jump check：跳跃检查\
    Backtracking：回溯，最大时间是400ms，开启后能够射击敌人的回溯，一般绿演开启\
    Current config：当前武器配置，下拉可选择不同武器，独立配置每个武器的参数
*   **Accuracy**

    Smooth：平滑度，范围为 **0.000\~50.000**，影响瞄准敌人的速度。部分武器会出现Smooth 2选项，此时Smooth的数值影响武器第一枪的效果，Smooth 2的数值影响第二枪及之后的效果\
    RCS：后坐力控制系统（Recoil Control System）的简称，开启后能够更改后坐力，也即软件协助压枪\
    RCS Pitch：后坐力控制的垂直角度，也即绕X轴，范围为 **0%\~50%**，数值越大后坐力效果越不明显\
    RCS Yaw：后坐力控制的水平角度，也即绕Y轴，范围为 **0%\~50%**，数值越大后坐力效果越不明显
*   **Target**

    FOV：视野角度，范围为 **0.000\~50.000**，只有当处于所设定的范围内legitbot才会工作。部分武器会出现FOV 2选项，此时FOV的数值影响武器第一枪的效果，FOV 2的数值影响第二枪及之后的效果\
    Shot delay：延迟射击，范围为 **0ms\~1000ms**，在所设定的时间后进行射击，用于模仿看见敌人后的反应时间\
    Kill delay：延迟击杀，范围为 **0ms\~1000ms**，击杀完敌人后在所设定的时间内继续进行射击，用于模仿确认击杀敌人的反应时间\
    Hitboxes：射击部位，一共有五个选项：**Head（头部）**、**Neck（脖子）**、**Pelvis（骨盆）**、**Stomach（腹部）**、**Chest（胸部）**，各个部位的伤害具体可见 [**csgo中的具体伤害计算**](https://www.bilibili.com/read/cv3164601/)
*   **Misc**

    Hitchance：命中率，影响射击敌人时的命中概率\
    Auto pistol：自动手枪，只有手枪才有此选项，开启后能够像步枪一样全自动射击\
    Recoil based FOV：根据视野角度调整后坐力，即智能压枪\
    Silent aim：静默瞄准，开启后射击时本地视角不会瞄准敌人\
    Auto fire：自动开火，可绑定键位，默认始终开启，开启后看见敌人自动射击\
    Aim at backtrack：回溯瞄准，有三个选项：**Disabled（关闭）**、**Nearest（距离准星最近的回溯）**、**Last（最后的回溯）**

#### ragebot <a href="#user-content-1.2" id="user-content-1.2"></a>

<figure><img src="../../../.gitbook/assets/image (28).png" alt=""><figcaption></figcaption></figure>



*   **Globals**

    Enable：开启暴力bot，可以绑定键位，默认始终开启。开启后全自动开枪，无后坐力，怎么暴力怎么来，一般在semirage和hvh中使用\
    Penetrate walls：穿墙，开启后会穿透墙体射击敌人，一般semirage关闭，hvh开启\
    Silent aim：静默瞄准，开启后射击时本地视角不会瞄准敌人，一般hvh开启\
    Desync correction：假身修正，也即俗称的解析器，会计算敌人的假身情况对真身进行射击。一般来说解析器是衡量一个cheat好坏的标准，**但是请记住IQ > ALL，解析器不能代表一个cheat的所有**\
    FOV：视野角度，范围为 **0.000\~180.000**，只有当处于所设定的范围内ragebot才会工作。一般semirage数值较低，hvh直接拉到最大\
    Active exploit：开启漏洞，开启后会利用tickrate系统的bug来实现一些非常规操作。目前有且仅有两种模式：**Double tap（DT 双发）** 和 **Hide shots（HS 不抬头）**。当开启DT时，能够在1 tick时间内射出两发子弹，变相加快开枪速度。但是由于扩散的存在，会对准确率有一定的影响。对于单发武器如SSG 08和AWP，DT效果会变成射出一发子弹后teleport（闪现），因此配合autopeek功能可以快速击杀敌人，并有可能不掉血（取决于对手的开枪速度）。还有很重要的一点就是DT需要**recharge（充能）**，并且会**禁用fakelag**（使得fakelag在0 \~ 2范围内波动）。DT可以在官方服务器中使用，但是更多的是用于hvh服务器中。当开启HS时，能够取消on shot（抬头）状态，从而使得当你开枪时不会被敌人抓抬头，大大减少被爆头的几率，但是开启后开枪速度会稍稍减慢，并且同样的会**禁用fakelag**（使得fakelag在0 \~ 2范围内波动）。**DT和HS不能同时开启。**\
    Current config：当前武器配置，下拉可选择不同武器，独立配置每个武器的参数
*   **Accuracy**

    Hitchance：命中率，范围为 **0%\~100%**，影响射击敌人时的命中概率\
    Auto stop：自动急停，用于减小扩散，增加命中率\
    Auto scope：自动开镜，只有拥有瞄准镜的武器有此选项，用于减小扩散，增加命中率
*   **Target**

    Hitscan：射击部位，一共有六个选项：**Head（头部）**、**Pelvis（骨盆）**、**Stomach（腹部）**、**Chest（胸部）**、**Legs（腿部）**、**Foot（脚部）**，各个部位的伤害具体可见\
    Min damage：最低伤害，影响射击时造成的伤害和开枪速度\
    Safe points：安全部位，一共有三个选项：**Default（默认）**、**Prefer（偏向于）**、**Force（强制）**，优先级从小到大\
    Max misses：最大空枪数，影响开枪速度\
    Head point scale：头部多点边缘，影响开枪优先射击的部位\
    Body point scale：身体多点边缘，影响开枪优先射击的部位

#### antihit <a href="#user-content-1.3" id="user-content-1.3"></a>

<figure><img src="../../../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>



*   **Fakelag**

    Enable：开启假卡，开启时敌人会看见你几帧几帧移动，用于防止敌人攻击\
    Disable while：选择什么时候关闭假卡，有且只有一个选项：**Standing（站立时）**\
    Limit：假卡最大tick，范围为 **0\~14**，在官方服务器中大于6 tick时会回弹\
    Triggers：其它触发情况，有两个选项：**On peek（在peek时）**、**In air（在空中）**\
    Trigger limit：在其它触发情况下假卡的最大tick，范围为 **0\~14**
*   **Fake angles**

    Enable：开启假身，开启后能够利用漏洞使得敌人只能看到你的假身模型，防止真身被击中\
    Pitch：假身垂直角度，也即绕X轴，一共有三个选项：**Down（向下）**、**Zero（水平）**、**Up（向上）**\
    Base yaw：假身水平角度，也即绕Y轴，一共有三个选项：**Backwards（背对）**、**Left（朝左）**、**Right（朝右）**，能够进行藏头（将头的位置设置在墙体的后面来防止爆头）\
    At targets：对准目标，开启后假身会对准敌人所在的方向，防止视野外敌人轻松攻击头部\
    Desync length：假身距离，影响假身分离距离，不同距离效果不同\
    Switch desync side：切换假身方向，可绑定按键，默认切换开启
*   **Extra**

    Jittermove：抖动移动，开启后在移动时身体会抖动，防止被爆头\
    Fakeduck：假蹲，可绑定键位，默认按住开启。开启后会开启fakelag并快速蹲下站起，使得自己以蹲下的姿态实现站立的射击范围，多用于高低差防止爆头。**注意开启假蹲后无法使用DT/HS**\
    Autopeek：自动peek，可绑定键位，默认按住开启。开启后开枪会快速回到初始的位置，多用于SSG 08和AWP，并配合DT使用\
    Slowwalk：慢走，俗称假走，开启后能够缓慢行走，配合假身jitter更好地防止被爆头\
    Slowwalk speed：慢走速度，范围为 **0%\~100%**，调节慢走时的速度\
    Leg movement：腿部动作，有两个选项：**Never Slide（从不滑步）**、**Always Slide（始终滑步）**。多配合static leg（固定腿）拓展使用，防止在peek时敌人先打脚

#### visuals <a href="#user-content-1.4" id="user-content-1.4"></a>

<figure><img src="../../../.gitbook/assets/image (6) (2).png" alt=""><figcaption></figcaption></figure>



*   **ESP**

    Enable：开启透视\
    Box：显示框框\
    Name：显示名字\
    Weapon name：显示武器名字\
    Weapon icon：显示武器图标\
    Ammo：显示弹药\
    Health：显示生命值\
    Skeleton：显示骨骼\
    Hit skeleton：显示击中骨骼\
    History skeleton：显示回溯骨骼\
    Multipoints：显示边缘\
    Armor：显示护甲值\
    Sound：显示声音\
    Glow：模型发光\
    Flags：敌人状态\
    Arrows：显示箭头\
    Size：显示大小\
    Distance：显示距离\
    Time in dormant：透视休眠时间\
    Use server sounds：使用服务器声音
*   **Colored models**

    Enable：开启模型上色\
    Behind wall：墙后模型颜色\
    Material：上色类型\
    Ragdoll chams：布偶上色，此处布偶是指布偶模型，与身体部位有关\
    Disable model occlusion：关闭模型阻挡，开启后不显示墙体后的模型
*   **Misc**

    Watermark：开启水印\
    OBS bypass：绕过OBS\
    Spectators：开启观众\
    Force crosshair：强制准星\
    Draw aimbot FOV：绘制准星范围\
    Penetration crosshair：穿墙准星\
    Grenade prediction：手雷轨迹预测\
    Thirdperson：第三人称视角\
    Force thirdperson：强制第三人称视角\
    Nightmode：夜晚视觉\
    Hitmarker：击中标记\
    Hit sound：击中音效\
    Kill sound：击杀音效\
    No scope：消除开镜黑边，有两个选项：**Stalic（静态）**、**Dynamic（动态）**\
    Removals：屏蔽内容

#### skins <a href="#user-content-1.5" id="user-content-1.5"></a>

<figure><img src="../../../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>



*   **Skinchanger**

    Knife/Gloves/Weapons：刀/手套/武器皮肤修改\
    Model：对应模型\
    Wear：磨损，范围为 **0.001\~1.000**\
    Seed：模板，范围为 **0\~1000**\
    StatTrak：击杀计数器，范围为 **-1\~999999**\
    点击Apply应用
*   **Knife/Gloves/Weapons paintkit**

    由于数目过大，皮肤中英文对应请自行百度，寻找想要的模板请善用搜索功能
*   **Extra**

    Agent CT：警方干员模型\
    Agent T：匪方干员模型\
    Override view FOV：第一人称视野，范围为 **0.000\~150.000**\
    Aspect ratio：屏幕拉伸，范围为 **0.000\~5.000**\
    Viewmodel editor：手臂模型修改\
    Viewmodel X：手臂X轴，范围为 **-20.000\~20.000**\
    Viewmodel Y：手臂Y轴，范围为 **-20.000\~20.000**\
    Viewmodel Z：手臂Z轴，范围为 **-20.000\~20.000**\
    Viewmodel roll：手臂旋转，范围为 **-180.000\~180.000**\
    Viewmodel FOV：手臂视野，范围为 **0.000\~180.000**

#### lua <a href="#user-content-1.6" id="user-content-1.6"></a>

<figure><img src="../../../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>

*   **Scripts/Scripts items**

    详见[拓展（Lua）使用](https://github.com/EPCN-fla/Nixware-Instruction/wiki/\[CN]-Nixware-%E4%BD%BF%E7%94%A8%E6%89%8B%E5%86%8C#2)
*   **Action**

    Load script：加载脚本\
    Reload all：重新加载所有脚本\
    Unload all：卸载所有脚本\
    Refresh：刷新脚本列表

#### misc <a href="#user-content-1.7" id="user-content-1.7"></a>

<figure><img src="../../../.gitbook/assets/image (17) (2).png" alt=""><figcaption></figcaption></figure>



*   **Movement**

    Bunnyhop：自动连跳，俗称bhop\
    Autostrafer：自动加速，开启后在空中自动加速\
    Fast stop：快速急停\
    Fast duck：快速下蹲，利用漏洞消除蹲伏耐力\
    Jump bug：跳跃漏洞，可绑定键位，默认始终开启\
    Edge jump：边缘跳跃，可绑定键位，默认始终开启
*   **Miscellaneous**

    Clantag：组名\
    Unlock hidden convars：解锁隐藏convars\
    Unlock hidden convars：解锁作弊convars\
    Unlock inventory access：解锁库存切换\
    Show MM ranks：显示官匹段位\
    Show enemy money：显示敌人金钱\
    Auto accept：自动接受比赛\
    Overwatch revealer：监管显示双方信息\
    Remove severside ads：移除服务器广告\
    Antidll bypass：反DLL绕过VAC\
    Ping spike：假延迟
*   **Settings**

    Load/Save/Refresh：加载/保存/刷新cfg\
    New config name：新cfg名称\
    Create and save：创建并保存\
    Unload cheat：卸载作弊
