[mirai-core](../index.md) / [net.mamoe.mirai](./index.md)

## Package net.mamoe.mirai

### Types

| Name | Summary |
|---|---|
| [Bot](-bot/index.md) | 机器人对象. 一个机器人实例登录一个 QQ 账号. Mirai 为多账号设计, 可同时维护多个机器人.`abstract class Bot : CoroutineScope, `[`LowLevelBotAPIAccessor`](-low-level-bot-a-p-i-accessor/index.md)`, BotJavaFriendlyAPI, `[`ContactOrBot`](../net.mamoe.mirai.contact/-contact-or-bot/index.md) |
| [BotFactory](-bot-factory/index.md) | 构造 [Bot](-bot-factory/-bot.md) 的工厂. 这是 [Bot](-bot-factory/-bot.md) 唯一的构造方式.`interface BotFactory` |
| [LowLevelBotAPIAccessor](-low-level-bot-a-p-i-accessor/index.md) | [Bot](-bot/index.md) 相关协议层低级 API.`interface LowLevelBotAPIAccessor` |

### Annotations

| Name | Summary |
|---|---|
| [LowLevelAPI](-low-level-a-p-i/index.md) | 标示这个 API 是低级的 API.`annotation class LowLevelAPI` |

### Extensions for External Classes

| Name | Summary |
|---|---|
| [kotlinx.coroutines.CoroutineScope](kotlinx.coroutines.-coroutine-scope/index.md) |  |

### Properties

| Name | Summary |
|---|---|
| [supervisorJob](supervisor-job.md) | 获取 [Job](#) 的协程 [Job](#). 此 [Job](#) 为一个 [SupervisorJob](#)`val `[`Bot`](-bot/index.md)`.supervisorJob: CompletableJob` |

### Functions

| Name | Summary |
|---|---|
| [alsoLogin](also-login.md) | 登录, 返回 [this](also-login/-this-.md)`suspend fun <B : `[`Bot`](-bot/index.md)`> B.alsoLogin(): B` |
| [Bot](-bot.md) | 使用指定的 [配置](-bot.md#net.mamoe.mirai$Bot(net.mamoe.mirai.BotFactory, net.mamoe.mirai.utils.Context, kotlin.Long, kotlin.String, kotlin.Function1((net.mamoe.mirai.utils.BotConfiguration, kotlin.Unit)))/configuration) 构造 [Bot](-bot/index.md) 实例`fun `[`BotFactory`](-bot-factory/index.md)`.Bot(context: `[`Context`](../net.mamoe.mirai.utils/-context/index.md)`, qq: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`, password: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, configuration: `[`BotConfiguration`](../net.mamoe.mirai.utils/-bot-configuration/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Bot`](-bot/index.md)<br>`fun `[`BotFactory`](-bot-factory/index.md)`.Bot(context: `[`Context`](../net.mamoe.mirai.utils/-context/index.md)`, qq: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`, password: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html)`, configuration: `[`BotConfiguration`](../net.mamoe.mirai.utils/-bot-configuration/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Bot`](-bot/index.md)<br>自动加载现有协议的 [BotFactory](-bot-factory/index.md), 并使用指定的 [配置](-bot.md#net.mamoe.mirai$Bot(net.mamoe.mirai.utils.Context, kotlin.Long, kotlin.String, net.mamoe.mirai.utils.BotConfiguration)/configuration) 构造 [Bot](-bot/index.md) 实例`fun Bot(context: `[`Context`](../net.mamoe.mirai.utils/-context/index.md)`, qq: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`, password: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, configuration: `[`BotConfiguration`](../net.mamoe.mirai.utils/-bot-configuration/index.md)` = BotConfiguration.Default): `[`Bot`](-bot/index.md)<br>`fun Bot(context: `[`Context`](../net.mamoe.mirai.utils/-context/index.md)`, qq: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`, password: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, configuration: `[`BotConfiguration`](../net.mamoe.mirai.utils/-bot-configuration/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Bot`](-bot/index.md)<br>`fun Bot(qq: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`, password: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, configuration: `[`BotConfiguration`](../net.mamoe.mirai.utils/-bot-configuration/index.md)` = BotConfiguration.Default): `[`Bot`](-bot/index.md)<br>`fun Bot(qq: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`, password: `[`String`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)`, configuration: `[`BotConfiguration`](../net.mamoe.mirai.utils/-bot-configuration/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Bot`](-bot/index.md)<br>`fun Bot(context: `[`Context`](../net.mamoe.mirai.utils/-context/index.md)`, qq: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`, passwordMd5: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html)`, configuration: `[`BotConfiguration`](../net.mamoe.mirai.utils/-bot-configuration/index.md)` = BotConfiguration.Default): `[`Bot`](-bot/index.md)<br>`fun Bot(context: `[`Context`](../net.mamoe.mirai.utils/-context/index.md)`, qq: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`, passwordMd5: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html)`, configuration: `[`BotConfiguration`](../net.mamoe.mirai.utils/-bot-configuration/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Bot`](-bot/index.md)<br>`fun Bot(qq: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`, passwordMd5: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html)`, configuration: `[`BotConfiguration`](../net.mamoe.mirai.utils/-bot-configuration/index.md)` = BotConfiguration.Default): `[`Bot`](-bot/index.md)<br>`fun Bot(qq: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`, passwordMd5: `[`ByteArray`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-byte-array/index.html)`, configuration: `[`BotConfiguration`](../net.mamoe.mirai.utils/-bot-configuration/index.md)`.() -> `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html)`): `[`Bot`](-bot/index.md) |
| [closeAndJoin](close-and-join.md) | 关闭这个 [Bot](-bot/index.md), 停止一切相关活动. 所有引用都会被释放.`suspend fun `[`Bot`](-bot/index.md)`.closeAndJoin(cause: `[`Throwable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-throwable/index.html)`? = null): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [containsFriend](contains-friend.md) | `fun `[`Bot`](-bot/index.md)`.containsFriend(id: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [containsGroup](contains-group.md) | `fun `[`Bot`](-bot/index.md)`.containsGroup(id: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`): `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |
| [getFriendOrNull](get-friend-or-null.md) | `fun `[`Bot`](-bot/index.md)`.getFriendOrNull(id: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`): `[`Friend`](../net.mamoe.mirai.contact/-friend/index.md)`?` |
| [getGroupOrNull](get-group-or-null.md) | `fun `[`Bot`](-bot/index.md)`.getGroupOrNull(id: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html)`): `[`Group`](../net.mamoe.mirai.contact/-group/index.md)`?` |
| [join](join.md) | 挂起协程直到 [Bot](-bot/index.md) 协程被关闭 ([Bot.close](-bot/close.md)). 即使 [Bot](-bot/index.md) 离线, 也会等待直到协程关闭.`suspend fun `[`Bot`](-bot/index.md)`.join(): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
| [recall](recall.md) | 撤回这条消息.`suspend fun `[`Bot`](-bot/index.md)`.recall(message: `[`MessageChain`](../net.mamoe.mirai.message.data/-message-chain/index.md)`): `[`Unit`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-unit/index.html) |
