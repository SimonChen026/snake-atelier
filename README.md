# 贪吃蛇 Atelier

这是一个单文件网页游戏。主入口是 `index.html`，现代浏览器直接打开就能玩。

## 本机打开

```bash
open index.html
```

## 发给朋友

把整个 `Agents` 文件夹压缩后发给朋友，朋友解压后双击 `index.html` 即可。

## 变成任何人都能点开的链接

### GitHub Desktop 发布

1. 用 GitHub Desktop 打开这个文件夹
2. 点 `Publish repository`
3. 仓库名可用 `snake-atelier`
4. 不要勾选 `Keep this code private`
5. 点 `Publish repository`

发布后进入仓库网页，打开 `Settings` -> `Pages`，把发布方式设为：

- Source: `Deploy from a branch`
- Branch: `main`
- Folder: `/ (root)`

点 `Save` 后等待 1-3 分钟。网址通常是：

```text
https://你的用户名.github.io/仓库名/
```

例如：

```text
https://SimonChen026.github.io/snake-atelier/
```

### Netlify Drop

也可以打开 `https://app.netlify.com/drop`，把这个文件夹拖进去，等它生成网址。

也可以发布到 Vercel、Netlify 或任何静态网站托管服务。只要服务能识别根目录的 `index.html`，就能直接打开游戏。
