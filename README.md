# NextStop AI

面向大模型研究的论文检索与论文可视化提示词 Skill。

## Skills

两个 Skill 使用相同的六部分结构：任务目标、输入与默认值、执行流程、质量要求、输出要求、交付前检查。每个目录只包含 `SKILL.md`，没有附带脚本、参考文件或额外依赖配置。

| Skill | 用途 | 提示词 |
| --- | --- | --- |
| `paper-search` | 筛选过去 72 小时内兼具实质创新与真实外部关注的大模型论文 | [SKILL.md](skills/paper-search/SKILL.md) |
| `paper-visualization` | 将论文制作成多页海报、高清 PNG 和可直接发布的宣传文字 | [SKILL.md](skills/paper-visualization/SKILL.md) |

可将对应目录安装到支持 `SKILL.md` 的环境中，也可直接使用文件中的提示词。执行任务所需的联网、论文读取、浏览器渲染和文件导出能力由运行环境提供。

## 品牌资源

品牌资源统一存放在 `assets/`。

| 文件名 | 内容 | 状态 |
| --- | --- | --- |
| `logo.png` | 不带文字的图形 logo | 已加入，保留原文件 |
| `logo.svg` | 图形 logo 的 SVG 版本 | 待提供 |
| `logo-with-text.png` | 带文字的 logo | 待提供 |
| `logo-with-text.svg` | 带文字 logo 的 SVG 版本 | 待提供 |

后续版本按上述文件名加入；当前不生成占位图或自动描摹版本。
