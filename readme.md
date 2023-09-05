# 学习Rust 

## 认识Cargo

cargo 提供了一系列的工具，从项目的建立、构建到测试、运行直至部署，为 Rust 项目的管理提供尽可能完整的手段。同时，与 Rust 语言及其编译器 rustc 紧密结合，可以说用了后就忘不掉，如同初恋般的感觉。

### 创建项目

``` rust
cargo new world_hello
cd world_hello
```

上面的命令使用 cargo new 创建一个项目，项目名是 world_hello ，该项目的结构和配置文件都是由 cargo 生成，意味着我们的项目被 cargo 所管理。

早期的 cargo 在创建项目时，必须添加 --bin 的参数, 现在的版本，已经无需此参数，cargo 默认就创建 bin 类型的项目，顺便说一句，Rust 项目主要分为两个类型：bin 和 lib，前者是一个可运行的项目，后者是一个依赖库项目。

