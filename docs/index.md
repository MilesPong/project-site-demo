---
# https://vitepress.dev/reference/default-theme-home-page
layout: home

hero:
  name: "VitePress Demo"
  text: "现代化文档站点"
  tagline: 使用 VitePress + GitHub CI/CD 构建的高性能静态网站
  actions:
    - theme: brand
      text: 快速开始
      link: /guide/getting-started
    - theme: alt
      text: API 文档
      link: /api/
  image:
    src: /logo.svg
    alt: VitePress

features:
  - title: 🚀 极速启动
    details: 基于 Vite 构建，开发服务器启动速度飞快，热更新几乎是即时的
  - title: 📝 Markdown 支持
    details: 使用 Markdown 编写内容，支持 YAML Frontmatter、代码高亮等特性
  - title: 🎨 美观主题
    details: 内置精美的默认主题，支持暗色模式、导航栏、侧边栏等
  - title: ⚡ CI/CD 集成
    details: 配置 GitHub Actions 自动构建和部署到 GitHub Pages
  - title: 🔍 SEO 友好
    details: 自动生成规范链接、Sitemap，支持 Open Graph 标签
  - title: 📱 响应式设计
    details: 完美适配桌面和移动设备，提供优秀的阅读体验
---

## 快速示例

```bash
# 安装依赖
npm install

# 启动开发服务器
npm run docs:dev

# 构建生产版本
npm run docs:build
```
