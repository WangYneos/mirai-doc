[mirai-core](../../../index.md) / [net.mamoe.mirai.event.events](../../index.md) / [BotOfflineEvent](../index.md) / [Active](./index.md)

# Active

`data class Active : `[`BotOfflineEvent`](../index.md)`, `[`BotActiveEvent`](../../-bot-active-event.md)`, CauseAware`

主动离线. 主动广播这个事件也可以让 [Bot](../../../net.mamoe.mirai/-bot/index.md) 关闭.

### Constructors

| Name | Summary |
|---|---|
| [&lt;init&gt;](-init-.md) | 主动离线. 主动广播这个事件也可以让 [Bot](../../../net.mamoe.mirai/-bot/index.md) 关闭.`Active(bot: `[`Bot`](../../../net.mamoe.mirai/-bot/index.md)`, cause: `[`Throwable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-throwable/index.html)`?)` |

### Properties

| Name | Summary |
|---|---|
| [bot](bot.md) | `val bot: `[`Bot`](../../../net.mamoe.mirai/-bot/index.md) |
| [cause](cause.md) | `val cause: `[`Throwable`](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-throwable/index.html)`?` |
