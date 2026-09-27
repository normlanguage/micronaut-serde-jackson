# Micronaut Serialization 示例

[English](README.md) | [简体中文](README.zh-CN.md)

[类型化 JSON 往返](sample/serde/Main.norm)是独立的消费者模块：把带注解的 `Message` 序列化为 JSON，再反序列化为 `Message`，输出两次结果。[示例模块](sample/serde/module.norm)声明完整依赖；[库模块](../micronaut/serde/jackson/module.norm)指定 Jackson 实现。

在仓库根目录运行：

```sh
norm run samples/sample/serde/Main.norm
```

预期程序输出：

```text
{"text":"Norm"}
Norm
```

Micronaut 也可能在标准错误输出中提示没有安装 SLF4J provider。
