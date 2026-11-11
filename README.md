# dsh-plugins-core

DSH **核心 / 基础设施插件包**：CAE 桥、HTTP 网关保活补丁、桌宠同步、手机远程连接。

## 内容

| 插件 | 包名 | 作用 | 来源 |
| --- | --- | --- | --- |
| `cae-bridge` | `@local/dsh-cae-bridge` | CAE/CAD 工具桥：MATLAB / Abaqus / COMSOL / AutoCAD | 自研（MIT） |
| `keepalive` | `@local/dsh-webserver-keepalive` | 拉长宿主 HTTP 网关 keepAliveTimeout，消除半死 socket | 自研（MIT） |
| `crosspet` | `@local/dsh-plugin-crosspet` | CrossPet 桌宠状态与余额同步 | 自研 |
| `dsh-remote-plugin` | `dsh-remote-plugin` | 手机/远程连接 + 内置网关 + 管理台 | 衍生自 Blank-not-black/dsh-Remote（MIT） |

## 未入库

- `dsh-remote-plugin/apk/`（10 MB APK 二进制）按「二进制不入库」规则排除；需要时从上游仓库 [Blank-not-black/dsh-Remote](https://github.com/Blank-not-black/dsh-Remote) 下载。

## 许可与第三方

`dsh-remote-plugin` 为 MIT，并内嵌 GSAP / morphicons / jsQR 三个第三方运行时；逐项见 **`THIRD_PARTY_NOTICES.md`**。

## 可见性

当前为 **Private**。判定依据见知识库 `CaiGouPlus/dsh-tiddlywiki` 的笔记「仓库拆分与隐私分级规范」：
涉及本机指纹、账号/订阅身份、IM 桥接、个人创作、NSFW 的内容一律私有。

## 恢复方式

把对应目录拷回本机后重启 DSH：
- 插件 → `D:\DSH\<插件名>`（`crosspet` 例外：`%LOCALAPPDATA%\CrossPet\dsh-plugin-crosspet`）
- 技能 → `%USERPROFILE%\.dsh\skills\<技能名>`
- 若插件在 profile 里以 `link:` 挂载，恢复后确认 `%USERPROFILE%\.dsh\profiles\desktop` 的链接仍指向上述路径。
