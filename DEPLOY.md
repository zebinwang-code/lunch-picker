# 部署指南

## 推荐：Cloudflare Pages（国内访问更快）

纯静态站，零配置，直接连 GitHub 仓库自动部署。

### 步骤

1. 访问 [pages.cloudflare.com](https://pages.cloudflare.com)，登录账号
2. 点 **Create application → Pages → Connect to Git**
3. 选择 `zebinwang-code/lunch-picker` 仓库
4. 构建配置留空（无需 build command，output directory 填 `.`）
5. 点 **Save and Deploy**，等 30 秒即可

部署完成后得到 `*.pages.dev` 链接，每次 push 到 `main` 自动重新部署。

### 国内访问说明

- `*.pages.dev` 域名在国内可访问，但偶有被墙。
- 绑定自定义域名后稳定性更好（Cloudflare 后台 → Custom domains）。
- 如需更稳定的国内访问，需要自定义域名 + ICP 备案，走 Cloudflare 中国合作网络。

---

## 备用：Vercel

### 拖拽部署

1. 访问 [vercel.com/drag-drop](https://vercel.com/drag-drop)
2. 把 `lunch-picker` 文件夹拖进去，等待部署
3. 得到 `xxx.vercel.app` 链接

### GitHub 连接部署

1. 访问 [vercel.com](https://vercel.com) → New Project → 选 `lunch-picker` 仓库 → Deploy

---

## 本地运行

```bash
cd lunch-picker
python3 -m http.server 8080
# 访问 http://localhost:8080
```
