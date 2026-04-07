# 🎮 OptikLink 保活

使用 Playwright + GitHub Actions 自动登录 OptikLink，保持免费服务器在线。

## ⚙️ 配置步骤

### 1️⃣ Fork 或上传此仓库到 GitHub

### 2️⃣ 添加 Secrets

进入仓库 → **Settings** → **Secrets and variables** → **Actions** → **New repository secret**：

| 🔑 Secret 名称 | 📝 格式 | ✅ 必填 |
|---|---|---|
| `DISCORD_ACCOUNT` | `email,password` | ✅ |
| `PANEL_ACCOUNT` | `username,password` | ✅ |
| `TG_BOT` | `chat_id,bot_token` | 可选 |
| `GOST_PROXY` | `socks5://user:pass@host:port` | 可选 |

### 3️⃣ 启用 Actions

进入 **Actions** 标签页，点击 **Enable GitHub Actions**。

### 4️⃣ 手动触发测试

**Actions** → **🎮 OptikLink 保活** → **Run workflow**

## 🕐 运行时间

每 **2 天** UTC 01:00（北京时间 9:00）自动运行。

可在 `.github/workflows/optiklink.yml` 的 `cron` 表达式中修改。
