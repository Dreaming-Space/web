# 帮助

## 设定

* 默认规划五大主城（东、南、西、北、中），其他城镇村落均由玩家自行协商、规划。
* 不权限干涉玩家正常生存。
* 自由市场经济。
* 游戏内的各项税收和服务费用（自杀命令除外）均会计入系统余额，用于每日的签到和经济成长奖励。*玩家支付的税费和各项服务费用最终会通过签到等奖励流回玩家市场*。

## 怎样获取节操

1. 领取在线奖励。
2. 在商城出售物品。
3. 自己动手，丰衣足食。
    * 选择一种途径获取基础物资：
        * 成为农民，大量种植农作物；
        * 成为矿工，在*荒野*挖掘各种矿石；
        * 成为怪物猎人。
    * 去中城交易所寻找收购员，出售物资，获得「绿宝石」。
    * 将「绿宝石」拿在手中，执行 `/sell hand` 即可获得节操。

## 插件

服务器中各类插件提供的命令用法及使用命令所消耗的金钱。请注意使用命令*消耗的是游戏内货币「节操」*，节操*不需要充值*，可以在游戏中通过各种合法渠道获得。插件仅用于提供有限的便利，即便不使用任何辅助插件的命令也可以正常生存。

### Essentials

*  `/spawn` 可以回到出生点。
*  `/sethome` 设置家，躺下可以设置床（死亡返回或 `/home bed` 返回），设置床不收取费用，计费方式：
    * 在主世界中心的价格为 500 节
    * 距离主世界中心越远，价格越低。每增加 1000 格距离降低 100 节
    * 最低价格为 50 节
    * 跨世界传送另收取 10 节
*  `/home` 传送回家，计费方式：
    * 起步价 10 节
    * 距离 home 点距离越远价格越高，每 1000 格距离增加 10 节
    * 最高收费 50 节
    * 跨世界传送另收取 10 节
*  `/back` 回到上一次传送点，计费方式：
    * 起步价 20 节
    * 距离 back 点距离越远价格越高，每 1000 格距离增加 20 节
    * 最高收费 100 节
    * 跨世界传送另收取 10 节

### 木牌锁

* 直接在箱子上、门上、贵重方块上贴木牌即可快速锁上该方块。
* 右键点击锁上的木牌后可以使用 `/lock [行号] [文字]` 来修改木牌。只有第 3、4 行是可以被修改的。例如 `/lock 3 Notch` 即可为玩家 `Notch` 添加对该木牌的权限。
* 如果不希望使用箱子锁而只是为了在箱子（或其他可被锁上的方块，例如门或钻石块等）上贴上木牌，可以按住 `shift` 再贴上即不会触发快捷锁。

### 在线时间统计

*  `/ptt` 查看自己的游戏时间。
* 满足在线时间规则执行 `/ptt ac` 即可获得奖励。
    * 每日在线 1 分钟可获得系统余额 1% 奖励
    * 每日在线 1 小时可获得系统余额 2% 奖励
    * 每日在线 3 小时可获得系统余额 5% 奖励
    * 每周在线 10 小时可获得系统余额 10% 奖励
    * 每月在线 30 小时可获得系统余额 10% 奖励

### Capcat 传送牌

* 使用鼠标对准欲购买的传送牌，使用 `/cc tp create [名称] [世界] [x] [y] [z] [价格]` 可购买未被使用的传送牌，需要执行 `/cc tp create confirm` 确认。
* 传送费用将进入传送牌所有者账户（收取 10% 所得税）。

### NyaaUtils 游戏辅助

* `/nu format` 查看允许使用的样式代码。
* `/nu prefix [前缀]` 消耗 100 节和 100 经验更改前缀。
* `/nu suffix [后缀]` 消耗 100 节和 100 经验更改后缀。
* `/nu rename [名称]` 消耗 10 点经验和 物品数量 * 5节重命名物品。支持格式代码。
* `/nu show` 在聊天区展示主手中正在持有的物品。鼠标移动到该行文本即可查看属性。
* 创建快递箱：`/nu mailbox create` 并右键点击箱子。
* 移除快递箱：`/nu mailbox remove`。
* 查看自己的快递箱信息：`/nu mailbox info`。
* 将主手中的物品发送给目标玩家(价格 1 节/次)：`/nu mailbox send [目标玩家 ID]`，例如将 20 个面包发送给玩家 `Notch` 则手持 20 个面包并输入 `/nu mailbox send Notch`。
* 将一箱物品发送给目标玩家(价格 20 节/箱)：`/nu mailbox sendchest [目标玩家 ID]` 并右键点击要发送的箱子。
* 火药可以用作飞行动力。将火药放在背包中，展开鞘翅滑翔时速度低于一定程度即可消耗火药来加速，从而保持飞行状态。由此可实现各种飞行特技，或长时间低空飞行游览世界。每次加速会消耗 1 个火药，当鞘翅耐久或火药即将用尽时会有提示。使用命令 `/nu el` 可切换此功能的开启或关闭状态，即便不使用火药依然可以实现原版的鞘翅滑翔。
* 经验存储：手持经验瓶，输入 `/nu expcap store [数量]` 即可将相应数量的经验存储到经验瓶。如果要恢复一定数量的经验，则手持存有经验的经验瓶，使用 `/nu expcap restore [数量]` 命令。如果将存有经验的经验瓶打碎，那么存储的经验会在瓶子破碎的方块重新生成。存储后的经验瓶不绑定玩家，可用于交易等。
* 在游戏中输入 `@[玩家 ID]` 可提及其他玩家，或者 `@[空格][玩家ID]` 用于 Tab 补全。例如 `@ Notch` 则该玩家在游戏中将收到提示。

### 投票

* 发起投票： `/nu vote [主题] [选项1] [选项2] …` 例如 `/nu vote 今晚吃什么 面包 烤鱼 蛋糕 企鹅`
* 参与投票： `/nu vote [选项ID]` 例如 `/nu vote 1` 投票给第一项。

### 叮咚商城

* 将物品拿在手上，使用 `/hm [单价]` 在叮咚商城销售物品，例如手持一组羊毛输入 `/hm 1` 即可以每个羊毛 1 节的价格上架一组羊毛。每位玩家可以占用最多 10 个物品槽。
* `/hm` 查看叮咚商城中的物品。左键点击购买一个，`shift + 左键` 点击购买全部。
* 使用 `/hreq [物品] [单价] [数量]` 收购物品。例如以 1 节的单价收购 100 个羊毛则输入 `/hreq wool 1 100`。
* 将物品拿在手上，使用 `/hauc [起步价] [步进价] [保留价]` 拍卖手上的物品。例如以底价 100 节，每次抬价至少 10 节拍卖附魔书，且希望至少拍到 150 节才出售，则将要拍卖的附魔书拿在手上，输入 `/hauc 100 10 150` 即可。如果不设置保留价格（即只要有人出价成功即可购得），使用 `/hauc 100 10`。
* 叮咚商城的上架费用（即每次 `/hm [单价] 的费用`）为 1 节，销售价格为原价 + 5% 税。上架后每三次元 24 小时时间收取 1 节的托管费用，直到物品售出。
* 叮咚商城的每次成功拍卖，均会收取成交价格的 10% 作为手续费用。
* `heh` 相关的命令，均可以将鼠标移动到消息文字上来预览物品，查看详细属性。

### 木牌商店

* 每位玩家可以创建最多 10 个木牌商店，包括销售、收购和乐透（抽奖）。
* 每位玩家的销售和收购商店木牌最多可以共享 128 个物品槽的空间。*请注意，同一玩家的同类型商店木牌内容是同步一致的，请善用此特性。*
* 乐透和收购木牌的存储箱不占用物品槽限制。*存储箱使用设置命令可以覆盖，即箱子可以之后重新设置到不和木牌在同一位置的地方。新的存储箱将立即生效，但之前箱子里的物品不会转移到新的箱子。*
* 木牌交易消费税 2%。
* 木牌格式：
    * 销售物品
        * 第一行 `[shop]`
        * 第二行 `SELL`
        * 第三行和第四行任意文本
        * 手中拿着需要上架出售的物品，准星对准木牌，命令 `/heh shop sell [单价]`。例如 1 节每个的价格上架一组羊毛，则手持一组羊毛 `/heh shop sell 1`
    * 收购物品
        * 第一行 `[shop]`
        * 第二行 `BUY`
        * 第三行和第四行任意文本
        * 创建牌子后，使用命令 `/heh shop storage set` 然后右键点一个箱子设置收购用存储箱。收购的物品将存储在此箱子中。
    * 乐透/抽奖
        * 第一行 `[shop]`
        * 第二行 `LOTTO`
        * 第三行 任意文本
        * 第四行 单次交易价格
        * 创建牌子后，使用命令 `/heh shop lotto set` 然后右键点一个箱子设置抽奖池。请将物品放在此箱子中，每次交易将从中随机抽取 1 个槽的物品。
* 如希望搜索木牌商店中正在销售的物品，请使用 `/heh search [关键字]` 进行搜索，例如 `/heh search wood` 。

### 叮咚直送

* 以特定总价向特定玩家销售手中的物品。例如向玩家 miu 以 100 节的总价销售手中的 12 个面包：`/hsellto miu 100`。买家将收到相应的账单 ID 通知，支付账单后，货物即发送给买家。
* 支付账单 `/hpay [invoice ID]` 例如 `/hpay 12345` 注意 ID 不是款项，请认真阅读账单包含的物品内容和款项。
    * 注意：账单 ID 并非私密，也并非只有买家才能支付特定账单。
* 直送的消费税是 2%，每位玩家最多可以有 20 份等待支付的卖方账单。
* 其他帮助信息：`/heh transaction help`
