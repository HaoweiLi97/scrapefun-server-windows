# ScrapeFun Server for Windows

[产品主页](https://github.com/HaoweiLi97/ScrapeFun) · [稳定版下载](https://github.com/HaoweiLi97/scrapefun-server-windows/releases/latest) · [全部发行](https://github.com/HaoweiLi97/scrapefun-server-windows/releases) · [在线文档](https://scrapefun.com/#/docs)

> 文档更新：2026-09-28。下列版本和资产为核对当日的稳定版；后续以对应 Release 为准。

Windows 系统托盘宿主，内置 ScrapeFun Server，通过默认浏览器提供管理界面。用于管理影视、漫画与 WebDAV / AList 远程媒体库，也可供局域网中的 Client 连接。

## 下载与系统环境

| 项目 | 当前稳定版 |
| --- | --- |
| 版本 | [0.3.3](https://github.com/HaoweiLi97/scrapefun-server-windows/releases/tag/v0.3.3) |
| 架构 | x64 |
| 首次安装 | `ScrapeFunServer-stable-Setup.exe` |
| 更新资产 | `releases.stable.json`、`ScrapeFunServer-0.3.3-stable-full.nupkg` |

从[稳定版下载页](https://github.com/HaoweiLi97/scrapefun-server-windows/releases/latest)下载 setup。首次安装不要选择 nupkg；系统要求和发布者签名状态以具体安装包及 Release 为准。

## 安装与首次启动

1. 运行 setup，完成安装并启动 Server。
2. 在系统托盘打开 ScrapeFun 网页界面，默认地址为 `http://127.0.0.1:8096`。
3. 新实例按网页引导设置管理员凭据并添加存储与媒体库。
4. 需要其他设备连接时，再启用局域网访问并检查防火墙。

已有实例继续使用原有账号。不要把历史版本的初始密码日志流程当作所有新版本的初始化方式。

## 托盘与数据目录

托盘菜单提供打开网页、重启服务、查看数据与日志目录、开机启动、局域网访问以及更新检查等入口。

运行数据默认位于：

```text
%APPDATA%\ScrapeFunDesktop
```

业务数据位于 `data`，日志位于 `logs`。这些数据在安装目录之外；更新安装程序通常不会删除它们。主动清理用户数据目录会影响整个实例，操作前先备份。

## 更新与旧安装迁移

当前使用 Velopack 管理 stable / beta 更新。可从网页设置或托盘检查更新，也可运行新版 setup。更新会重启服务，应先暂停任务并导出备份。

旧 Inno Setup 安装需要先退出并卸载旧宿主，再运行一次 Velopack setup。保留 `%APPDATA%\ScrapeFunDesktop`，迁移后检查登录、媒体库和数据；之后可使用应用内更新。

## 故障排查

服务打不开时检查进程、端口占用、托盘中的日志目录和防火墙。反馈时提供 Windows 版本、Server 版本、安装方式及脱敏日志。

## 支持与授权

本仓库提供平台安装说明和官方发行资产。使用问题与功能建议请提交到[主仓库 Issues](https://github.com/HaoweiLi97/ScrapeFun/issues)；账号、激活或私密日志请联系 `scrapefun@outlook.com`。报告安全问题请按[安全说明](./SECURITY.md)私密提交。

新的商业许可声明见 [LICENSE](./LICENSE)，完整条款见[软件使用许可协议](./EULA.md)。个人、家庭及组织内部可正常使用；Pro 需有效授权，软件再分发、转售、客户交付和收费托管须单独书面授权。该声明不追溯改变既有授权；现有资产以其随包许可为准，第三方组件继续适用各自许可证。

[发行与兼容性说明](https://github.com/HaoweiLi97/ScrapeFun/blob/main/RELEASE_POLICY.md) · [第三方组件说明](https://github.com/HaoweiLi97/ScrapeFun/blob/main/THIRD_PARTY_NOTICES.md) · [支持流程](./SUPPORT.md)
