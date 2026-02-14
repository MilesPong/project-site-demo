# 快速开始

本指南将帮助你快速了解如何使用 VitePress 创建文档站点。

## 前置要求

- [Node.js](https://nodejs.org/) 18 或更高版本
- 包管理器（npm、yarn 或 pnpm）

## 安装

### 使用 npm

```bash
npm install
```

## 启动开发服务器

```bash
npm run docs:dev
```

VitePress 将在本地启动开发服务器，默认地址是 `http://localhost:5173`。

## 项目结构

```
.
├── docs/
│   ├── .vitepress/
│   │   └── config.mjs          # 站点配置
│   ├── guide/
│   │   ├── getting-started.md  # 本文件
│   │   └── configuration.md    # 配置说明
│   ├── api/
│   │   └── index.md            # API 文档
│   └── index.md                # 首页
├── .github/
│   └── workflows/
│       └── deploy.yml          # CI/CD 配置
└── package.json
```

## 添加新页面

1. 在 `docs` 目录下创建 Markdown 文件
2. 在 `docs/.vitepress/config.mjs` 中添加导航或侧边栏链接

## 构建生产版本

```bash
npm run docs:build
```

构建输出将生成在 `docs/.vitepress/dist` 目录。

## 预览生产构建

```bash
npm run docs:preview
```

## 下一步

- 查看 [配置说明](./configuration) 了解更多配置选项
- 访问 [VitePress 官方文档](https://vitepress.dev/) 获取完整指南
