# tiny-ui — Tiny 家族设计系统

本文件是 **Google Stitch** 读取的设计系统入口,用于统一生成 Tiny 家族 4 个产品的前端界面。

---

## 设计原则

唯一规范来源:**Material Design 3**([m3.material.io](https://m3.material.io/))

涵盖范围:sys-color / ref-palette / typescale / shape / elevation / motion / state / 组件结构 / light & dark scheme。

---

## 产品主色

每个产品指定 1 个 source color,M3 算法自动派生完整 sys-color(light / dark 两套)。

| 产品 | Source color | Hex | Scheme | 主题 |
|------|--------------|-----|--------|------|
| tiny-dashboard | Indigo 500 | `#6366f1` | Content-based | Light |
| tiny-ems       | Emerald 500 | `#10b981` | Content-based | Light |
| tiny-shop      | Amber 500 | `#f59e0b` | Content-based | Light |
| tiny-dfm       | Emerald 500 | `#10b981` | **Fidelity** | **Dark** |

> 色名(Indigo / Emerald / Amber)仅作人类可读标识,实际以 hex 为准。

### M3 dynamic color 说明

- `source color`:你指定(见上表)
- `primary / secondary / tertiary`:算法从 source color 派生
- `error`:M3 内置(固定红橙系)
- `neutral / neutral-variant`:算法派生的灰阶
- `surface / on-surface / outline`:由 neutral 派生

---

## 使用方式

1. 打开 [stitch.withgoogle.com](https://stitch.withgoogle.com/)
2. 新建项目时,导入本 `DESIGN.md`
3. Stitch 按 M3 规范、并以上表主色 / 主题为基准生成界面

各产品项目落地时,使用 [Material Theme Builder](https://material-foundation.github.io/material-theme-builder/) 输入对应 source color 与 scheme,导出 CSS 变量 / JSON tokens 后集成进项目。
