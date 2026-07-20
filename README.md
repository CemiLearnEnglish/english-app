# ⭐ 宝宝学英语 - 儿童幼升小英语学习App

面向5-6岁儿童的交互式英语学习网页应用，帮助从幼儿园到小学顺利过渡。

## 功能模块

| 模块 | 说明 |
|------|------|
| 🔤 **字母学习** | A-Z 26个字母，点击卡片学发音和单词 |
| 📚 **单词认知** | 动物、颜色、数字、水果、身体 5大分类 |
| 🎤 **大声朗读** | 看→听→读 三步互动，语音识别检测跟读 |
| 🧠 **趣味测验** | 10题一轮，看图选词/中英配对 |
| 🏆 **我的成就** | 星星和进度追踪 |

## 部署到 GitHub Pages

### 方法一：使用 GitHub CLI（推荐）

```bash
# 1. 进入项目目录
cd english-app

# 2. 初始化 Git 仓库
git init
git add .
git commit -m "初始化英语学习App"

# 3. 在 GitHub 创建仓库（替换 YOUR_USERNAME 为你的GitHub用户名）
gh repo create english-app --public --source=. --remote=origin --push

# 4. 开启 GitHub Pages
gh api repos/YOUR_USERNAME/english-app/pages -X POST -f source.branch=main -f source.path=/
```

### 方法二：手动部署

1. 在 GitHub 上新建仓库（如 `english-app`）
2. 本地运行：
   ```bash
   git init
   git add .
   git commit -m "初始化英语学习App"
   git remote add origin https://github.com/你的用户名/english-app.git
   git push -u origin main
   ```
3. 进入仓库 Settings → Pages → 选择 `main` 分支，`/` (root) 目录 → Save
4. 等待几分钟，你的App将出现在 `https://你的用户名.github.io/english-app/`

## 平板使用

1. 在平板浏览器打开 GitHub Pages 链接
2. 点击浏览器菜单 → "添加到主屏幕"
3. 之后可离线使用，像原生App一样全屏运行

## 本地使用

直接用浏览器打开 `index.html` 即可，无需安装任何依赖。