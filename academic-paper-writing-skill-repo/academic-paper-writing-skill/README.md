# academic-paper-writing — 学术论文写作约束 Skill

一个面向 Claude 的 [Agent Skill](https://docs.claude.com)，把一整套**学术研究论文写作的规则、约束与检查清单**内化进模型。
它不只是"讲解"写作概念，而是让 Claude 在**帮你写、改、审、评**论文时，主动按这些规则执行。

> 本 Skill 的内容根据萨克雷大学（Sacred Heart University）图书馆研究指南
> *Organizing Academic Research Papers*（基于南加州大学 USC 图书馆 Dr. Robert V. Labaree 的材料）
> **用我们自己的语言重新提炼、改写**而成，并非原文照搬。详见 [`NOTICE`](./NOTICE)。

---

## ✨ 功能特性

- **贯穿全文的通用原则**：单一研究问题驱动、论点先行、证据支撑、正式精确语气、术语谨慎、引用一切非原创内容。
- **按论文结构逐节的约束**，覆盖完整的核心写作流程：
  研究设计 → 选题与研究问题 → 标题 → 提纲 → 段落 → 摘要 → 引言 → 文献综述 →
  方法 → 结果 → 讨论 → 局限性 → 结论 → 校对 → 引用与避免抄袭。
- **两个按需加载的参考文件**：学术风格细则 + 常见语法错误速查 + 引用/抄袭规则；以及更深入的分节细节与各类分类法。
- **最终质量检查清单**：交稿前对照自检。

## 🎯 适用场景（自动触发）

只要你在规划、起草、修改、批改任何学术论文、学位论文、期刊文章、课程论文、研究计划或文献综述时，
即使只提一句——

- "帮我看看这段摘要写得对不对"
- "我的研究问题好不好？"
- "把讨论部分收紧一点"
- "方法部分应该写什么？"
- "怎么让这段文字更学术、更正式？"
- "怎么避免抄袭 / 怎么校对？"

——Claude 都会启用本 Skill，并把相应约束**应用到实际写作/审阅中**。

## 📦 目录结构

```
academic-paper-writing-skill/
├── README.md                          # 本文件
├── LICENSE                            # MIT（仅覆盖本仓库的封装与改写表达）
├── NOTICE                            # 来源与版权声明（重要）
├── .gitignore
├── academic-paper-writing/           # 可直接安装的 skill 目录
│   ├── SKILL.md                      # 主文件：工作流 + 通用原则 + 逐节约束 + 检查清单
│   └── references/
│       ├── section-reference.md         # 各章节深入细节与分类法
│       └── style-grammar-citation.md    # 学术风格 / 语法速查 / 引用与抄袭
└── dist/
    └── academic-paper-writing.skill  # 打包好的可安装文件
```

## 🚀 安装方法

**方式一：直接安装打包文件（推荐）**

1. 下载 [`dist/academic-paper-writing.skill`](./dist/academic-paper-writing.skill)。
2. 在 Claude 应用中打开 **Settings → Capabilities → Skills**，上传该 `.skill` 文件即可。

**方式二：使用源文件**

把 `academic-paper-writing/` 整个目录放入你的 skills 目录，或在 Claude Code / Claude Cowork 项目中按其文档加载。

> 想自己重新打包，可使用官方 skill-creator 的打包脚本：
> `python -m scripts.package_skill <skill 目录> <输出目录>`

## 🧩 适用范围说明

本 Skill 聚焦于**论文写作核心流程**（约 22 个原指南页面提炼而来）。
原指南中与"写论文"关系不大的内容——口头报告、小组项目管理、书评、田野报告、政策备忘录，
以及纯查阅类页面（术语表、内容提醒服务、延伸阅读清单）——**未包含**在内。
如需加入，欢迎提交 PR。

## 📚 来源与署名

- 原始内容：Sacred Heart University Library, *Organizing Academic Research Papers*
  （基于 USC Libraries, Dr. Robert V. Labaree, *Organizing Your Social Sciences Research Paper*）。
- 本仓库内容为对上述材料的**独立提炼与改写**，用于教学辅助目的，并保留对原作者与机构的署名。
- 具体请阅读 [`NOTICE`](./NOTICE)。

## 📄 许可

本仓库**自身的表达、封装与组织方式**以 [MIT 许可](./LICENSE) 发布。
请注意：MIT 仅覆盖本仓库作者贡献的部分，**不构成**对底层原始指南版权的再授权。
使用、再分发前请阅读 [`NOTICE`](./NOTICE) 并自行判断合规性。本仓库不提供法律意见。

## 🤝 贡献

欢迎通过 Issue / PR 改进规则措辞、补充章节或修正错误。提交时请勿粘贴原指南的整段原文，
保持"用自己的话提炼"的原则。
