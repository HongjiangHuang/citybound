### First Day.

第一天主要粗略的阅读了 browser_ui 的代码. 弄明白了该项目是使用 rust wasm + react 来实现的前端.

由于不是很明白 rust + wasm 来作为前端的开发如何跟react混合编译. 所以我补充了 rust wasm 相关的知识.

[[Repo分享]rust+wasm，关于这一切](https://rust.cc/article?id=03616001-275b-4e0e-9b4f-a2b8fdfbd53f)

通过这个文章我大致的明白了. 在开发的过程中. rust 如何跟 JavaScript 交互.
譬如
```
// 导入 JS 函数 `foo`
extern { fn foo(); }

// 导出 Rust 函数 `bar`
#[no_mangle]
pub extern fn bar() {
  // TODO::...
}
```

[以及rust 如何跟旧的npm 生态兼容](https://github.com/rustwasm/team/issues/5).