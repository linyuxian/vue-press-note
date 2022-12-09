---
lang: zh-CN
title: ESLint
description: 页面的描述
---

# ESLint

[ESLint](https://eslint.org/) 是一个根据方案识别并报告 ECMAScript/JavaScript 代码问题的工具，其目的是使代码风格更加一致并避免错误。在很多地方它都与 JSLint 和 JSHint 类似，除了：

- ESLint 使用 [Espree](https://github.com/eslint/espree) 对 JavaScript 进行解析。
- ESLint 在代码中使用 AST 评估方案。
- ESLint 完全是插件式的，每个规则都是一个插件，你可以在运行时中添加更多插件。

## ESLint 配置

你可以根据你的情况定制 ESLint，它十分灵活且具可配置性。你可以关闭全部规则，只运行基本的语法验证，或者也可以根据项目需要，一起使用合适的捆绑规则与自定义规则。主要有两个配置 ESLint 的方法：

1. 配置注释 - 在文件中使用 `JavaScript` 注释直接嵌入配置信息

2. 配置文件 - 使用 `JavaScript`、`JSON` 或 `YAML` 文件指定整个目录及其所有子目录的配置信息。可以是 `.eslintrc.\*` 文件，也可以是 `package.json` 文件中的 `eslintConfig` 字段，ESLint 都会自动寻找并读取这两处的配置，或者还可以用命令行上指定配置文件。

下面列出了一些 ESLint 中可配置的选项：

- [环境](https://zh-hans.eslint.org/docs/latest/user-guide/configuring/language-options#specifying-environments) - 你的脚本被设计为在哪些环境下运行。每个环境都会附带一组预设的全局变量。
- [全局变量](https://zh-hans.eslint.org/docs/latest/user-guide/configuring/language-options#specifying-globals) - 脚本在执行过程中需要用到的额外全局变量。
- [规则](https://zh-hans.eslint.org/docs/latest/user-guide/configuring/rules) - 启用了哪些规则，它们又是什么级别错误水平
- [插件](https://zh-hans.eslint.org/docs/latest/user-guide/configuring/plugins) - 第三方插件为 ESLint 定义了额外的规则、环境、配置等。

所有这些选项使得你可以对 ESLint 处理代码的模式进行进准控制。
