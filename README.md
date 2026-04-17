# APOS 跨境新零售商城文档

基于 MkDocs Material 主题构建的 APOS 商城系统在线文档。

## 🚀 本地开发

### 安装依赖
```bash
pipx install mkdocs-material --include-deps
```

### 本地预览
```bash
mkdocs serve
```
访问 http://127.0.0.1:8000

### 构建静态文件
```bash
mkdocs build
```
构建结果在 `site/` 目录

## 📦 部署到 Cloudflare Pages

### 方式一：通过 GitHub 自动部署

1. 推送代码到 GitHub
2. 登录 [Cloudflare Dashboard](https://dash.cloudflare.com/)
3. 进入 **Pages** → **Create a project**
4. 选择 **Connect to Git**
5. 选择你的 GitHub 仓库
6. 配置构建设置：
   - **Build command**: `mkdocs build`
   - **Build output directory**: `site`
7. 点击 **Save and Deploy**

### 方式二：通过 Wrangler CLI 部署

```bash
# 安装 Wrangler
npm install -g wrangler

# 登录 Cloudflare
wrangler login

# 部署
wrangler pages deploy site --project-name=apos-docs
```

## 📝 文档结构

```
docs/
├── index.md              # 首页
├── 商城入门/             # 商城基础配置
├── 商品管理/             # 商品规格、价格、运费
├── 支付配置/             # 支付方式设置
├── 订单管理/             # 发货、收货、售后
├── 营销功能/             # 扫码购、直播、推广
└── 跨境业务/             # 清关、保税业务
```

## 🔧 配置说明

主要配置文件：`mkdocs.yml`

- 站点名称、描述
- 主题颜色
- 导航结构
- 搜索配置
- Markdown 扩展

## 📚 相关链接

- [MkDocs 官方文档](https://www.mkdocs.org/)
- [Material for MkDocs](https://squidfunk.github.io/mkdocs-material/)
- [APOS 官方文档](http://docs.jieztech.com/jiedoc/)

## 📄 许可证

Copyright © 2026 APOS 技术支持
