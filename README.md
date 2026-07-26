# ScrapeFun Server for Windows

> 最后更新：2026 年 7 月 26 日

ScrapeFun Server for Windows 将服务端和系统托盘宿主整合为一个安装程序，适合直接在 Windows 电脑上运行媒体库服务。

## 下载

从 [Releases](https://github.com/HaoweiLi97/scrapefun-server-windows/releases/latest) 下载最新的 `x64-setup.exe`，双击完成安装。

## 首次启动

安装后 ScrapeFun 会在系统托盘运行。双击托盘图标可用默认浏览器打开管理界面。

首次启动生成的初始密码会写入日志。右键托盘图标并选择 `Show Logs Directory`，即可打开日志目录查看。

## 托盘菜单

托盘菜单可用于：

- 打开 ScrapeFun
- 重启服务
- 查看数据目录和日志目录
- 设置开机启动
- 开启或关闭局域网访问
- 检查 stable 或 beta 更新

## 数据与日志

运行数据默认保存在：

```text
%APPDATA%\ScrapeFunDesktop
```

日志位于其中的 `logs` 子目录。卸载应用不会自动删除用户数据；重新安装后仍可继续使用原有数据。

## 应用内更新

新版使用 Velopack 管理 stable 和 beta 更新。旧版 Inno 安装用户需要先退出并卸载旧宿主，再手动安装一次新版 setup；之后即可使用应用内更新。

## 相关链接

- [ScrapeFun 使用与 Docker 文档](https://github.com/HaoweiLi97/ScrapeFun)
- [macOS Server](https://github.com/HaoweiLi97/scrapefun-server-macos)
- [产品网站](https://mightly.store/)
