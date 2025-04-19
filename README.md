# gfast-ci-lint

<div align="center">

[![Go Report Card](https://goreportcard.com/badge/github.com/gfast-ci-lint)](https://goreportcard.com/report/github.com/gfast-ci-lint)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Go Version](https://img.shields.io/badge/go-1.21+-00ADD8.svg)](https://golang.org/dl/)
[![Release](https://img.shields.io/github/v/release/gfast-ci-lint?include_prereleases&style=flat-square)](https://github.com/gfast-ci-lint/releases)

</div>

<div align="center">

## 🚀 预告：gfast 框架即将推出！ 🚀

</div>

> gfast 是一款全新的 Go 语言微服务开发框架，专注于提供高性能、易用性和扩展性。框架采用模块化和插件化设计，让开发者能够根据实际需求灵活组装功能模块。
>
> 在技术实现上，gfast 基于 gRPC 和 HTTP/2 构建服务治理体系，支持多样化的服务发现机制，并提供统一的配置管理中心。框架内置了分布式链路追踪和监控告警系统，为微服务运维提供全方位支持。
>
> 为提升开发体验，gfast 配备了完善的工具链，包括项目脚手架、代码生成器和调试工具。框架提供丰富的内置组件，真正实现"开箱即用"。详尽的文档和示例确保开发者能快速上手。
>
> 无论是构建小型服务还是大规模微服务集群，gfast 都能满足开发者的需求，是构建现代化微服务应用的理想选择。
>
> ⭐️ 敬请期待！ ⭐️

<div align="center">

## ✨ 特性

</div>

- 🛡️ 严格的代码质量检查
- 📝 统一的代码风格规范
- 🤖 自动化的代码审查
- ⚙️ 可配置的检查规则

## 配置说明

本配置包含以下主要检查项：

- `errcheck`: 检查未处理的错误
- `goimports`: 自动格式化导入语句
- `govet`: 代码静态分析
- `staticcheck`: 高级静态分析
- `gocognit`: 代码复杂度检查
- `funlen`: 函数长度检查
- `cyclop`: 循环复杂度检查
- `gosec`: 安全检查
- `nestif`: 嵌套 if 语句检查
- `maintidx`: 可维护性指数检查
- `godox`: 代码注释检查
- `decorder`: 声明顺序检查

## 使用说明

1. 安装 golangci-lint：

```bash
go install github.com/golangci/golangci-lint/cmd/golangci-lint@latest
```

2. 将 `.golangci.yml` 配置文件复制到项目根目录

3. 运行检查：

```bash
golangci-lint run
```

## 配置参数说明

### 复杂度检查
- `gocognit`: 最小复杂度阈值 10
- `cyclop`: 最大复杂度 12，包平均复杂度 11
- `funlen`: 函数最大行数 60，最大语句数 40

### 代码规范
- `decorder`: 声明顺序为 type -> const -> var -> func
- `godox`: 检查特殊注释标记（NOTE, OPTIMIZE, HACK）
- `maintidx`: 可维护性指数阈值 30
- `nestif`: if 语句最小复杂度 3

## 贡献指南

欢迎提交 Issue 和 Pull Request 来改进这个规范。

## 许可证

MIT License
