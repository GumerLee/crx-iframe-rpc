# crx-iframe-rpc

[![npm version](https://img.shields.io/npm/v/crx-iframe-rpc.svg)](https://www.npmjs.com/package/crx-iframe-rpc)
[![license](https://img.shields.io/npm/l/crx-iframe-rpc.svg)](./LICENSE)

[中文说明](./README.zh-CN.md)

> **Issue tracker only.** This repository does not host the source code and publishes no releases. `crx-iframe-rpc` is maintained independently by its author and distributed through npm; this repository exists so that users have a place to report bugs and request features.

Bridge Chrome extension APIs from a Chrome extension page into an embedded iframe — a zero-dependency RPC layer over `postMessage`.

## Install

```bash
pnpm add crx-iframe-rpc
# or
npm install crx-iframe-rpc
# or
yarn add crx-iframe-rpc
# or
bun add crx-iframe-rpc
```

The full usage guide, API reference and changelog ship inside the package and are rendered on the [npm package page](https://www.npmjs.com/package/crx-iframe-rpc). Please read them before opening an issue.

## Reporting a bug

Search the [existing issues](https://github.com/GumerLee/crx-iframe-rpc/issues) first. If nothing matches, open a new issue with the **Bug report** template and fill in every field:

- **Package version** — run `npm ls crx-iframe-rpc` (or `pnpm ls crx-iframe-rpc`). This repository has no tags or releases, so the version number is the only way to pin down what you are running.
- **Environment** — Chrome version, Manifest version (MV2 / MV3), where the host page lives (options page, popup, side panel, any `chrome-extension://` page) and where the iframe content is loaded from (the same extension, a web origin, a sandboxed frame, …).
- **Entry points in use** — `exposeChrome` / `connectChrome`, or the generic `serveRpc` / `connectRpc` / `serveRpcWithPoster`, plus any non-default options.
- **Steps to reproduce** — a minimal snippet or repository is ideal.
- **Expected vs. actual behavior**, including the complete error message or warning text.

## Requesting a feature

Open an issue with the **Feature request** template. Describe the use case first, then explain why the current API does not cover it. Suggestions for the API shape are welcome but optional.

## Security

Please do not report security problems in a public issue. Use **Report a vulnerability** under the repository's **Security** tab instead.

## What you will not find here

- Source code, pull requests, tags or releases — the code lives in the author's private repository.
- Usage docs — they are part of the package itself; see the npm page above.

## License

`crx-iframe-rpc` is released under the [Apache License 2.0](./LICENSE).
