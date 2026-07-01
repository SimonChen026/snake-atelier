# 贪吃蛇 Atelier

一个可以直接在浏览器运行的贪吃蛇网页游戏。项目不需要安装依赖，也不需要后端服务；打开 `index.html` 就能玩。

游戏支持桌面键盘和移动端触控。在 iPhone 上会显示拖动摇杆，蛇会按连续方向移动，可以平滑转弯并形成曲线蛇身。

## 在线试玩

GitHub Pages:

```text
https://simonchen026.github.io/snake-atelier/
```

## 本地运行

在 macOS 上可以直接运行：

```bash
open index.html
```

也可以双击 `index.html`。`snake.html` 是兼容入口，会自动跳转到主页面。

## 项目结构

- `index.html`: 游戏主文件，包含页面结构、样式和游戏逻辑
- `snake.html`: 旧入口兼容文件
- `.nojekyll`: 让 GitHub Pages 按普通静态文件发布
- `README.md`: 项目说明

## 发布到 GitHub Pages

仓库发布到 GitHub 后，进入仓库网页并打开 `Settings` -> `Pages`，设置为：

- Source: `Deploy from a branch`
- Branch: `main`
- Folder: `/ (root)`

保存后等待 1-3 分钟，网页通常会发布到：

```text
https://你的用户名.github.io/仓库名/
```

## 安全说明

这个项目是纯静态网页，不需要 API key、访问令牌、数据库密码或服务器密钥。

发布前请确认不要提交以下内容：

- `.env`、`.env.local` 等环境变量文件
- API key、access token、client secret
- 私钥文件，例如 `.pem`、`.key`
- 真实账号密码或个人隐私数据

当前游戏的账号和存档数据只保存在玩家自己的浏览器 `localStorage` 中，不会上传到服务器。以后如果接入第三方 API，请把密钥放在服务端，不要写进前端 HTML、CSS 或 JavaScript 文件里。
