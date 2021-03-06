[mirai-core](../../index.md) / [net.mamoe.mirai.event.events](../index.md) / [MessageRecallEvent](./index.md)

# MessageRecallEvent

`sealed class MessageRecallEvent : `[`BotEvent`](../-bot-event/index.md)`, `[`AbstractEvent`](../../net.mamoe.mirai.event/-abstract-event/index.md)

消息撤回事件. 可是任意消息被任意人撤回.

**See Also**

[Contact.recall](../../net.mamoe.mirai.contact/recall.md)

### Types

| Name | Summary |
|---|---|
| [FriendRecall](-friend-recall/index.md) | 好友消息撤回事件, 暂不支持.`data class FriendRecall : `[`MessageRecallEvent`](./index.md)`, Packet` |
| [GroupRecall](-group-recall/index.md) | 群消息撤回事件.`data class GroupRecall : `[`MessageRecallEvent`](./index.md)`, `[`GroupOperableEvent`](../-group-operable-event/index.md)`, Packet` |

### Properties

| Name | Summary |
|---|---|
| [authorId](author-id.md) | 消息原发送人`abstract val authorId: `[`Long`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-long/index.html) |
| [messageId](message-id.md) | 消息 id.`abstract val messageId: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) |
| [messageInternalId](message-internal-id.md) | 消息内部 id.`abstract val messageInternalId: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) |
| [messageTime](message-time.md) | 原发送时间`abstract val messageTime: `[`Int`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html) |

### Extension Properties

| Name | Summary |
|---|---|
| [isByBot](../is-by-bot.md) | `val `[`MessageRecallEvent`](./index.md)`.isByBot: `[`Boolean`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html) |

### Extension Functions

| Name | Summary |
|---|---|
| [__broadcastJava](../../net.mamoe.mirai.event/__broadcast-java.md) | 在 Java 广播一个事件的唯一途径.`fun <E : `[`Event`](../../net.mamoe.mirai.event/-event/index.md)`> E.__broadcastJava(): E` |
| [broadcast](../../net.mamoe.mirai.event/broadcast.md) | 广播一个事件的唯一途径.`suspend fun <E : `[`Event`](../../net.mamoe.mirai.event/-event/index.md)`> E.broadcast(): E` |
