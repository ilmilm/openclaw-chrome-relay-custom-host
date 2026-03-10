# OpenClaw Browser Relay (Custom Host)

Chrome extension for attaching OpenClaw to an existing Chrome tab via a CDP relay server — with **configurable host/IP + port**.

> 中文简介在下方（Chinese summary below）。

## Features
- Configure **Host/IP** and **Port** in Options
- Default: `127.0.0.1:18792`
- Stores Gateway token securely in extension local storage

## Install (Chrome)
1. Download or clone this repo.
2. Open `chrome://extensions`.
3. Enable **Developer mode**.
4. Click **Load unpacked** and select this folder.
5. Click the extension icon on the target tab to attach/detach.

## Configure
Open the extension **Options** page and set:
- **Host / IP**: e.g. `127.0.0.1` (local) or `10.0.0.177` (LAN)
- **Port**: Relay port (Gateway port + 3). Default `18792`
- **Gateway token**: must match `gateway.auth.token`

## Security Notes
- If you use a LAN IP, ensure your relay is properly secured.
- Anyone who can reach the relay + token can control the attached tab.

---

# OpenClaw Browser Relay（可自定义 Host/IP）

用于把 OpenClaw 接到已有 Chrome 标签页的扩展，支持**自定义 Host/IP + 端口**。

## 功能
- 在 Options 里配置 **Host/IP** 和 **Port**
- 默认 `127.0.0.1:18792`
- Token 保存在扩展本地存储

## 安装（Chrome）
1. 下载或克隆本仓库
2. 打开 `chrome://extensions`
3. 开启开发者模式
4. 选择“加载已解压的扩展程序”并选中本目录
5. 在目标标签页点击扩展图标即可连接/断开

## 配置
打开扩展 **Options** 页面，填写：
- **Host / IP**：如 `127.0.0.1`（本机）或 `10.0.0.177`（局域网）
- **Port**：Relay 端口（Gateway 端口 + 3），默认 `18792`
- **Gateway token**：必须与 `gateway.auth.token` 一致

## 安全提示
- 若使用局域网 IP，请确保 relay 访问安全
- 任何能访问 relay 且有 token 的人都能控制标签页

## License
MIT
