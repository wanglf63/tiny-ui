# tiny-ui — Tiny 家族设计系统

本文件是 **Google Stitch** 读取的设计系统入口,用于统一生成 Tiny 家族 4 个产品的前端界面。

## 设计原则

- 视觉语言遵循 **Material Design 3**([m3.material.io](https://m3.material.io/))
- 布局与工具类习惯参考 **Tailwind CSS**([tailwindcss.com](https://tailwindcss.com/))
- 设计 token、组件结构、动效、阴影等细节以以上两套规范为准,本文件不重复定义
- 本文件**只声明每个产品的主色与主题模式**,作为对默认规范的定制项

## 产品主色

主色取自 **Tailwind CSS** 色板。

| 产品 | 主色 token | 主题模式 |
|------|------------|----------|
| tiny-dashboard | `indigo-500` | Light |
| tiny-ems       | `emerald-500` | Light |
| tiny-shop      | `amber-500` | Light |
| tiny-dfm       | `emerald-500` | **Dark** |
