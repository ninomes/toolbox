# 工具导航 Toolbox

新装机必备工具导航页 —— 把常用软件官网一站找齐，点击直达下载。

## 本地预览

直接双击 `index.html` 即可，无需任何构建。

## 部署到 GitHub Pages

1. 在 GitHub 新建仓库，如 `toolbox`
2. 把 `index.html` 推到仓库：

```bash
git init
git add index.html README.md
git commit -m "init: 工具导航页"
git branch -M main
git remote add origin https://github.com/<你的用户名>/toolbox.git
git push -u origin main
```

3. 仓库设置 → **Settings → Pages** → Source 选 `Deploy from a branch`，Branch 选 `main` / `(root)`，保存
4. 1 分钟后访问 `https://<你的用户名>.github.io/toolbox/` 即可

## 如何新增工具

打开 `index.html`，在 `TOOLS` 数组里加一行：

```js
{ cat: "dev", name: "工具名", desc: "一句话说明", url: "https://官网", icon: "字" },
```

分类可选：`social` 社交聊天 / `browser` 浏览器 / `cloud` 网盘 / `media` 影视音乐 / `dev` 编程开发 / `office` 效率办公 / `ai` AI 助手。

## 待办

- [ ] `dsh` 的官网链接目前是 `#` 占位，补充真实地址
