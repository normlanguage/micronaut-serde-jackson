# Micronaut Serialization samples

[English](README.md) | [简体中文](README.zh-CN.md)

[Typed JSON round trip](sample/serde/Main.norm) is an independent consumer module. It serializes an annotated `Message` to JSON, deserializes it as `Message`, and prints both results. The [sample module](sample/serde/module.norm) declares its complete dependency set; the [library module](../micronaut/serde/jackson/module.norm) pins the Jackson implementation.

From the repository root, run:

```sh
norm run samples/sample/serde/Main.norm
```

Expected program output:

```text
{"text":"Norm"}
Norm
```

Micronaut may also warn on stderr that no SLF4J provider is installed.
