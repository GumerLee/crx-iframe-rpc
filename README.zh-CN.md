# crx-iframe-rpc

[![npm version](https://img.shields.io/npm/v/crx-iframe-rpc.svg)](https://www.npmjs.com/package/crx-iframe-rpc)
[![license](https://img.shields.io/npm/l/crx-iframe-rpc.svg)](./LICENSE)

[English](./README.md)

> **本仓库仅用于问题收集。** 这里不托管源码，也不发布 Release。`crx-iframe-rpc` 由作者独立维护并通过 npm 发布；建立本仓库只是为了给使用者一个反馈 bug、提出功能需求的地方。

把 Chrome 扩展 API 从 Chrome 扩展页桥接到内嵌的 iframe —— 一个基于 `postMessage` 的零依赖 RPC 层。

## 安装

```bash
pnpm add crx-iframe-rpc
# 或
npm install crx-iframe-rpc
# 或
yarn add crx-iframe-rpc
# 或
bun add crx-iframe-rpc
```

完整的使用指南、API 说明和更新日志都随包一起发布，可在 [npm 包页面](https://www.npmjs.com/package/crx-iframe-rpc) 直接阅读。提 issue 之前请先看一遍。

## 反馈 Bug

请先搜索[已有 issue](https://github.com/GumerLee/crx-iframe-rpc/issues)。确认没有重复后，用 **Bug report** 模板新建 issue，并填全每一项：

- **包版本**——运行 `npm ls crx-iframe-rpc`（或 `pnpm ls crx-iframe-rpc`）。本仓库没有 tag 和 Release，版本号是定位你所用代码的唯一依据。
- **环境信息**——Chrome 版本、Manifest 版本（MV2 / MV3）、宿主页所在位置（options 页、popup、side panel 或任意 `chrome-extension://` 页面），以及 iframe 内容的来源（同一扩展、Web 源、sandbox 帧等）。
- **使用的入口**——`exposeChrome` / `connectChrome`，还是通用层的 `serveRpc` / `connectRpc` / `serveRpcWithPoster`，以及改动过的非默认选项。
- **复现步骤**——最好附最小可复现的代码片段或仓库。
- **期望行为与实际行为**，附完整的报错或警告文本。

## 提功能需求

用 **Feature request** 模板新建 issue。先说明使用场景，再说明现有 API 为什么无法满足；如果对 API 形态有建议也欢迎写上，但不是必须。

## 安全问题

请不要在公开 issue 中报告安全问题，改用仓库 **Security** 标签页下的 **Report a vulnerability**。

## 这里没有的东西

- 源码、Pull Request、tag 和 Release——代码在作者的私有仓库中维护。
- 使用文档——文档在包内，见上文的 npm 页面。

## 许可证

`crx-iframe-rpc` 基于 [Apache License 2.0](./LICENSE) 发布。
