# 第三方组件与来源说明

## 一、衍生项目

| 本仓库路径 | 上游项目 | 原作者 | 许可 | 关系 |
| --- | --- | --- | --- | --- |
| `plugins/dsh-remote-plugin` | https://github.com/Blank-not-black/dsh-Remote | Blank-not-black | MIT | 手机/远程连接 + 内置网关 + 管理台，本机作为 bundle 插件使用 |

## 二、内嵌的第三方运行时

| 组件 | 上游 | 原作者 | 许可 | 位置 |
| --- | --- | --- | --- | --- |
| GSAP 3.15.0 | https://github.com/greensock/GSAP | GreenSock (Jack Doyle) | GreenSock Standard "No Charge" License（https://gsap.com/standard-license） | `plugins/dsh-remote-plugin/public/vendor/gsap/`（附 `NOTICE.md`） |
| morphicons 1.7.0 | https://github.com/guillermolg00/morphicons | Copyright (c) 2026 Guillermo | MIT | `plugins/dsh-remote-plugin/public/vendor/morphicons/`（附原 `LICENSE`） |
| jsQR | https://github.com/cozmo/jsQR | cozmo | Apache-2.0 | `plugins/dsh-remote-plugin/public/jsqr.min.js` |

> Apache-2.0 与 MIT 均要求保留版权与许可声明；完整许可文本见上游仓库。GSAP 的商用条款以其官方许可为准。

## 三、自研部分

`cae-bridge`、`keepalive`、`crosspet` —— 自研，按各目录 `package.json` 声明（多为 MIT）分发。

## 四、无法逐一确认的引用

**本仓库部分模块基于互联网开源项目与公开示例优化**；如权利人认为使用不当，请开 issue 指出具体路径，我会补署名或移除。

_最后更新：2026-11-11_
