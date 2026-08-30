---
title: rust_learning
date: 2026-04-11 22:55:16
categories:
  - 学习笔记
tags:
  - Rust
---

# Rust 语法学习示例

这是一套详细的 Rust 编程语言学习示例代码，每个语法点一个文件，配有详细的中文注释。

[下载代码](/downloads/code/rust_learning.zip)

## 📚 学习路线

### 入门基础

1. **01_hello_world.rs** - Hello World，print 宏，格式化输出
2. **02_variables.rs** - 变量声明、可变性、常量、类型转换
3. **03_functions.rs** - 函数定义、参数、返回值、递归
4. **04_control_flow.rs** - if-else、match、循环、模式匹配

### 核心概念

5. **05_ownership.rs** - 所有权规则、移动、克隆
6. **06_borrowing.rs** - 借用与引用、可变引用、生命周期
7. **07_structs.rs** - 结构体定义、方法、关联函数
8. **08_enums.rs** - 枚举定义、Option、Result、模式匹配

### 错误处理

9. **09_error_handling.rs** - panic!、Result、Option、自定义错误

### 泛型与 Trait

10. **10_generics.rs** - 泛型函数、泛型结构体、Trait Bound
11. **11_traits.rs** - Trait 定义、实现、默认实现、trait 对象
12. **12_lifetimes.rs** - 生命周期标注、生命周期省略规则

### 标准库集合

13. **13_collections.rs** - Vec、String、HashMap、HashSet、迭代器适配器

### 函数式特性

14. **14_iterators.rs** - 迭代器创建、适配器、消费者方法
15. **15_closures.rs** - 闭包语法、捕获机制、Fn traits

### 智能指针

16. **16_smart_pointers.rs** - Box、Rc、RefCell、Arc、Mutex

### 代码组织

17. **17_modules.rs** - 模块定义、pub 可见性、use 语句

### 测试

18. **18_testing.rs** - 单元测试、集成测试、断言宏、TDD

### 高级特性

19. **19_unsafe_rust.rs** - unsafe 块、原始指针、FFI、union
20. **20_advanced_features.rs** - 宏、类型系统、并发基础、高级特性总结

## 🚀 运行方式

### 方式一：单独编译运行

```bash
rustc 01_hello_world.rs -o hello
./hello
```

### 方式二：创建 Cargo 项目

```bash
cargo new rust_learning
cd rust_learning
# 将示例文件内容复制到 src/main.rs 或 src/lib.rs
cargo run
```

### 方式三：运行测试

```bash
rustc --test 18_testing.rs -o tests
./tests
```

## 📖 学习建议

1. **按顺序学习**：建议按照编号顺序学习，每个文件都建立在前一个文件的基础上

2. **动手实践**：每个概念都提供了示例，尝试修改代码观察结果

3. **阅读注释**：每个文件都有详细的中文注释，解释了代码的含义

4. **运行验证**：使用 `rustc filename.rs` 编译运行，验证理解

5. **结合官方文档**：
   - [The Rust Programming Language](https://doc.rust-lang.org/book/)
   - [Rust by Example](https://doc.rust-lang.org/rust-by-example/)

## 🔧 工具推荐

- **rustc**: Rust 编译器
- **cargo**: Rust 包管理器
- **rust-analyzer**: IDE 插件（VS Code、Vim 等）
- **rustfmt**: 代码格式化工具
- **clippy**: Rust linter

## 📝 文件说明

| 文件  | 主题         | 难度 |
| ----- | ------------ | ---- |
| 01-04 | 基础语法     | ⭐    |
| 05-08 | 核心概念     | ⭐⭐   |
| 09    | 错误处理     | ⭐⭐   |
| 10-12 | 泛型与 Trait | ⭐⭐⭐  |
| 13-15 | 函数式       | ⭐⭐   |
| 16-17 | 高级特性     | ⭐⭐⭐  |
| 18-20 | 生态工具     | ⭐⭐   |

## 🤝 贡献

欢迎提出改进建议和错误反馈！

## 📄 许可证

MIT License
