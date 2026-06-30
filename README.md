# AstrBot Plugin - 森空岛自动签到

[![Build and Release](https://github.com/Azincc/astrbot_plugin_skland/actions/workflows/release.yml/badge.svg)](https://github.com/Azincc/astrbot_plugin_skland/actions/workflows/release.yml)

适用于 AstrBot 的森空岛自动签到插件，支持明日方舟和终末地。用户发送 `/skdlogin` 后通过官方二维码扫码登录，插件会保存登录凭证，并在绑定成功后立即执行一次签到。

## 功能

- **skdlogin** (全部): 生成二维码，扫码登录并立即签到
- **skd** (群聊): 查看群内已绑定用户的签到状态
- **skd** (私聊): 查看自己的签到状态
- **skdlogout** (全部): 登出并移除账号绑定
- **skdusers** (全部): 查询用户统计，管理员可查看更详细信息

## 使用

### 登录与签到

1. 发送 `/skdlogin` 获取二维码
2. 使用森空岛、明日方舟或终末地扫码确认登录
3. 登录成功后插件会保存绑定信息，并自动执行一次签到
4. 之后可以发送 `/skd` 查看签到状态

### 自动签到

管理员可在 AstrBot 插件配置中开启自动签到，并设置每日执行时间、随机延迟和最大绑定用户数。

## 安装

### 方式一：从 Release 下载

1. 前往 [Releases](https://github.com/Azincc/astrbot_plugin_skland/releases) 页面
2. 下载最新的 `astrbot_plugin_skland-vX.X.X.zip`
3. 解压到 AstrBot 的 `plugins` 目录

### 方式二：使用 Git

```bash
cd /path/to/astrbot/plugins
git clone https://github.com/Azincc/astrbot_plugin_skland.git
```

## 依赖

插件依赖已在 `requirements.txt` 中列出，AstrBot 会自动安装。

## 许可

MIT License
