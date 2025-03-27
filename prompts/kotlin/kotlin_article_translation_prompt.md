---
description: 指导 AI 将 Kotlin 英文技术文章翻译成专业、准确、术语一致的中文技术文档，适用于中文开发者阅读
globs:
alwaysApply: false
---
<!-- modified: 2025-03-27 -->
# Kotlin 英文文章翻译指令

## 任务描述

你的任务是将我提供的 Kotlin 英文技术文章准确翻译成中文。请保持翻译的专业性和技术准确性，确保使用符合中文 Kotlin 开发社区习惯的术语和表达方式。翻译结果面向具有 Kotlin 基础知识的中文开发者。直接提供完整的中文翻译内容，无需添加额外说明或解释翻译过程。

## 具体要求

- 将英文文章翻译成地道、流畅、符合中文表达习惯的技术文档
- 严格保持原文的技术准确性、专业性和逻辑关系
- 代码块内容（包括代码、输出结果和注释）保留英文原样，不翻译
- Kotlin 专业术语处理：
  - 使用中文 Kotlin 社区或官方认可的术语翻译
  - 无官方中文翻译时保留英文原词（如："Lambda"等）
  - "nullable"/"non-null" 统一翻译为"可空"/"非空"
- 完整保留原文的段落结构、标题层级和格式
- 专有名词首次出现时采用"中文（英文）"的格式标注
  - 例如：协程（coroutine）、作用域函数（scope function）
- 确保整体翻译上下文连贯，避免逐句机械翻译导致的语义不通
- 当遇到无法确定含义的术语时，保留英文并用方括号标注可能的解释
- 输出格式：仅提供完整翻译内容，不包含翻译过程说明或其他额外注释

## 术语参考

### 推荐翻译术语

以下术语应翻译成对应的中文：

| 英文术语 | 中文翻译 |
|---------|---------|
| Coroutine | 协程 |
| Extension Function | 扩展函数 |
| Nullable/Non-null | 可空/非空 |
| Scope Function | 作用域函数 |
| Companion Object | 伴生对象 |
| Data Class | 数据类 |
| Inline Function | 内联函数 |
| Sealed Class | 密封类 |
| Higher-order Function | 高阶函数 |
| Property Delegate | 属性委托 |
| Collection | 集合 |
| Infix Notation | 中缀表示法 |
| Type Inference | 类型推断 |
| Destructuring Declaration | 解构声明 |
| Type Alias | 类型别名 |
| Lazy Initialization | 延迟初始化 |
| Smart Cast | 智能转换 |
| Reified Type | 具体化类型 |
| Property | 属性 |
| Suspend Function | 挂起函数 |
| Function Type | 函数类型 |
| Flow | 流 |
| Receiver | 接收者 |
| Extension Property | 扩展属性 |
| Type Parameter | 类型参数 |
| Delegation Pattern | 委托模式 |
| Safe Call Operator | 安全调用运算符 |
| Elvis Operator | Elvis 运算符 |
| Callable Reference | 可调用引用 |
| Range | 区间 |
| Sequence | 序列 |
| Variance | 型变 |
| Covariance | 协变 |
| Contravariance | 逆变 |
| SAM Conversion | SAM 转换 |
| Operator Overloading | 运算符重载 |
| Lateinit | 延迟初始化 |
| By Keyword | by 关键字 |
| Nothing Type | Nothing 类型 |
| Object Expression | 对象表达式 |
| Object Declaration | 对象声明 |
| Top-level Function | 顶层函数 |
| Top-level Property | 顶层属性 |
| Primary Constructor | 主构造函数 |
| Secondary Constructor | 次构造函数 |
| Initialization Block | 初始化块 |
| Typealias | 类型别名 |
| Named Parameter | 命名参数 |
| Default Parameter | 默认参数 |
| Trailing Lambda | 尾随 Lambda |
| Multiplatform | 多平台 |
| Coroutine Context | 协程上下文 |
| Dispatcher | 调度器 |
| Channel | 通道 |

### 保留原文术语

以下术语通常保留英文原文，无需翻译：

| 英文术语 | 使用方式 |
|---------|---------|
| Lambda | 直接使用 Lambda |
| Kotlin/Native | 直接使用 Kotlin/Native |
| Kotlin/JS | 直接使用 Kotlin/JS |
| Kotlin/JVM | 直接使用 Kotlin/JVM |
| Compose | 直接使用 Compose |
| Continuation | 直接使用 Continuation |
| StateFlow | 直接使用 StateFlow |
| SharedFlow | 直接使用 SharedFlow |
| ViewModel | 直接使用 ViewModel |
| LiveData | 直接使用 LiveData |
| Gradle | 直接使用 Gradle |
| Kotlin DSL | 直接使用 Kotlin DSL |
| KDoc | 直接使用 KDoc |
| KSP | 直接使用 KSP（Kotlin Symbol Processing） |
| KAPT | 直接使用 KAPT（Kotlin Annotation Processing Tool） |
| Kotlin Multiplatform Mobile (KMM) | 直接使用 KMM 或完整名称 |
| kotlinx | 各库名称保持原样，如 kotlinx.coroutines |
| Kotest | 直接使用 Kotest |
| Ktor | 直接使用 Ktor |
| Jetpack | 直接使用 Jetpack |
| Koin | 直接使用 Koin |
| Maven | 直接使用 Maven |
