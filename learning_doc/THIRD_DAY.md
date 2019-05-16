### Third Day.

第三天.阅读完 [kay_codegen](https://github.com/aeplay/kay_codegen) 我发现 原本我以为 `kay_auto.rs` 是作者写的. 然后用于编译还是干嘛的.
看完之后才明白. 原来 `kay_auto.rs` 是 kay_codegen 根据每个模块的规范自动生成的. 而这一切又要追溯到作者的另一个项目. [kay](https://github.com/aeplay/kay).
kay 是作者用rust 对 actor 模型实现的一个框架. 主要用于游戏系统中各个角色的通讯. 相关 actor 的优缺点可以查看其它文献. 本文就不深究了。
`kay_auto.rs` 会根据每个模块生成对应的 Actor 对象. 以及对应的消息 Msg。 具体细节后续继续阅读.

我本人对 actor 模型也只是了解。周末会做一些demo来加深 对这个模型的理解。以便我更快的阅读.

每天的时间有限. 以及我目前的rust能力阅读的速度也不会太快。

明天加油 ~
