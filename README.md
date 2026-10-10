# Codex Windows 启动动画

为 Windows Codex 提供窗口内启动动画：头像圆环 → 碎片散开 → 角色描线 → 彩色画面 → 进入应用并保留静态背景。

## 下载

**[下载 Windows 安装包](https://github.com/ljun2464/codex-startup-animation-windows/releases/latest/download/Codex-Animation-Windows.zip)**

[查看版本说明及校验文件](https://github.com/ljun2464/codex-startup-animation-windows/releases/latest)

## 使用

1. 下载 ZIP，将整个文件夹解压到固定位置，不要直接在压缩包里运行。
2. 双击 `Install.cmd`，创建桌面的“Codex 动画”快捷方式。
3. 完全退出 Codex，包括托盘中的后台实例。
4. 双击桌面的“Codex 动画”，观看约 12 秒开场动画。

`Esc` 跳过；`Ctrl+Alt+B` 更换图片、文字和背景强度，或恢复原外观。
`Preview.cmd` 可在浏览器预览；`Start-Codex.cmd` 可直接启动。
移动文件夹后，需要重新运行 `Install.cmd`。

## 环境与限制

- Windows 10/11、Windows PowerShell 5.1、已安装的 Microsoft Store `OpenAI.Codex` 应用。
- Node.js 22+；也会尝试查找 Codex 自带的 Node 运行时。
- 仅在 Codex 26.1002.7124.0 验证，其他版本可能需要适配。
- ZIP 包含可读源码，不包含 Codex 本体、账号、订阅、制作者的登录资料或聊天数据。
- 不修改官方安装包。通过只绑定 `127.0.0.1` 的调试端口临时接入动画；同机其他进程可能连接这个端口。
- 完全退出后从官方入口启动，可关闭本次动画接入与调试状态。
- 安装脚本已静态检查；尚未在其他电脑实机测试。

## 版本改动

Windows 桌面入口自动发现、OpenAI 签名验证、调试端口归属检查、桌面快捷方式安装，以及减少转场重绘、隐藏动画更新和线稿到图片突变的调整。

## 来源与权利说明

原项目：[panding999/codex-startup-animation](https://github.com/panding999/codex-startup-animation)。动画与默认素材来源、原说明保留在安装包的 `upstream/README.md` 中。

本项目是非官方 Windows 适配，与 OpenAI 无隶属关系。原仓库未指定代码开源许可证；角色素材权利归各自权利人。本仓库未为上游代码或素材授予额外许可，请勿将公开可下载视为商用或再分发授权。