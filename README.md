# 中午吃什么 🍽️

每天纠结吃什么？交给命运吧！

## 功能

- 🎲 随机抽签选择餐厅
- 🏪 9家餐厅合集
- 📱 手机扫码下单

## 部署到 Vercel

### 方法一：GitHub 部署（推荐）

1. 创建 GitHub 仓库，把代码上传
2. 访问 [vercel.com](https://vercel.com)
3. 用 GitHub 登录
4. 点击 "New Project" → 选择你的仓库
5. 点击 "Deploy"，等待完成
6. 得到可访问的 URL

### 方法二：Vercel CLI 直接部署

```bash
# 1. 安装 Vercel CLI
npm i -g vercel

# 2. 进入项目目录
cd lunch-picker

# 3. 登录并部署
vercel login
vercel
```

### 方法三：拖拽部署

1. 访问 [vercel.com/drag-drop](https://vercel.com/drag-drop)
2. 把 `lunch-picker` 文件夹拖进去
3. 自动部署完成

## 本地运行

```bash
cd lunch-picker
python3 -m http.server 8080
# 访问 http://localhost:8080
```