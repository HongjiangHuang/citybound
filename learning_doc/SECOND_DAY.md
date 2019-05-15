### Second Day.

第二天继续阅读了前端的实现. 发现了每个模块除了js文件以外还会有 `mod.rs` 和 `kay_auto.rs`.

于是发现了 前端的编译过程. 会先执行 `build.rs` 来编译rust代码输出wasm文件。

阅读了该项目作者的子项目 [kay_codegen](https://github.com/aeplay/kay_codegen) 目测这个项目是专门为citybound写的。用于编译rust项目.

kay_codegen 会遍历整个前端项目目录. 查找 `mod.rs` 文件. 学过rust的朋友们应该都知道。 `mod.rs` 文件是rust 的模块系统。目录中有 `mod.rs` 说明该目录是rust 的模块。而 `mod.rs` 是该模块的入口文件

kay_codegen 查找到 `mod.rs` 之后。 会将目录当成一个模块。随后载入目录中的 `kay_auto.rs`

具体如何载入模块中的js, 实现 js 跟 rust 的互动。还需要后续分析 kay_codegen 项目中的 [generators.rs](https://github.com/aeplay/kay_codegen/blob/master/src/generators.rs)

每天的时间有限. 以及我目前的rust能力阅读的速度也不会太快。

明天加油 ~
