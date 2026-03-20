# Vercel 部署指南

## 拖拽部署（最简单）

1. **打开 Vercel 拖拽页面**
   访问: https://vercel.com/drag-drop

2. **准备文件夹**
   把 `/Users/admin/Documents/lunch-picker` 文件夹压缩成 zip

3. **拖拽上传**
   把压缩包拖进去，等待部署

4. **获取链接**
   部署完成后会得到一个 `xxx.vercel.app` 的链接

---

## GitHub 部署

1. 创建 GitHub 仓库: https://github.com/new
   - 仓库名: `lunch-picker`
   - 设为 Public

2. 上传代码
   ```bash
   cd /Users/admin/Documents/lunch-picker
   git init
   git add .
   git commit -m "initial commit"
   git remote add origin https://github.com/你的用户名/lunch-picker.git
   git push -u origin main
   ```

3. 部署
   - 访问 https://vercel.com
   - New Project → 导入仓库
   - Deploy!

---

## 部署后

1. 会得到一个 URL，如: `lunch-picker.vercel.app`
2. 分享这个链接给同事即可使用
3. 可在 Vercel 后台绑定自定义域名