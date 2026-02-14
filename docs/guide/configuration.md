# 配置说明

VitePress 使用 `.vitepress/config.mjs` 文件进行站点配置。

## 基础配置

```javascript
import { defineConfig } from 'vitepress'

export default defineConfig({
  // 站点标题
  title: 'VitePress Demo',

  // 站点描述
  description: 'A demo site built with VitePress',

  // 部署的基础路径（GitHub Pages 需要）
  base: '/github-pages-demo/',
})
```

## 主题配置

### 导航栏

```javascript
export default defineConfig({
  themeConfig: {
    nav: [
      { text: '首页', link: '/' },
      { text: '指南', link: '/guide/getting-started' },
      {
        text: '下拉菜单',
        items: [
          { text: 'Item A', link: '/item-1' },
          { text: 'Item B', link: '/item-2' }
        ]
      }
    ]
  }
})
```

### 侧边栏

```javascript
export default defineConfig({
  themeConfig: {
    sidebar: {
      '/guide/': [
        {
          text: '指南',
          items: [
            { text: '快速开始', link: '/guide/getting-started' },
            { text: '配置说明', link: '/guide/configuration' }
          ]
        }
      ]
    }
  }
})
```

### 社交链接

```javascript
export default defineConfig({
  themeConfig: {
    socialLinks: [
      { icon: 'github', link: 'https://github.com/vuejs/vitepress' },
      { icon: 'twitter', link: 'https://twitter.com/vuejs' }
    ]
  }
})
```

## 更多配置选项

查看 [VitePress 配置参考](https://vitepress.dev/reference/site-config) 了解所有可用选项。
