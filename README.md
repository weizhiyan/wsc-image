# wsc-skill-image — AI 视觉创意专家

[![Claude Code](https://img.shields.io/badge/Claude-Code-black?logo=anthropic)](https://claude.ai/code)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> 把你脑子里模糊的画面，变成 AI 能精准执行的提示词。

不管是「画一张赛博朋克风海报」还是「帮我把这张照片改成电影感」，直接说需求就行——不用背命令，不用懂提示词语法。

---

## 🎯 作用与定位

大多数人用 AI 画图，卡在「不知道怎么描述」这一步。wsc-image 解决的就是这个问题：

1. **生图提示词** — 你说一句话，它给你一段经过 7 层结构优化的专业提示词，能直接用。
2. **视频分镜** — 描述一个场景或故事，输出完整分镜表和每个镜头的运镜提示词。
3. **参考图分析** — 上传一张你喜欢的图，它从风格、色调、光影、构图四个维度拆解。
4. **修图/P图** — 提供原图，说「换背景」「保留人物」，自动生成保护五官比例的修改指令。

---

## 🚀 四大应用场景

AI 会根据你说的话自动判断场景，不需要你手动指定：

| 场景 | 触发示例 | 输出重点 |
| :--- | :--- | :--- |
| **A. AI 绘图** | 「帮我画一张赛博朋克风的城市夜景」 | 7层提示词结构（主体、光影、材质等） |
| **B. 视频分镜** | 「做一个产品发布的视频提示词」 | 镜头设计表 + 动感运镜描述 |
| **C. 参考图分析** | 「参考这张图，画一个类似氛围的人像」 | 四维风格拆解 + 意图确认弹窗 |
| **D. 修图/P图** | 「把这张图的背景换成洱海，保留人物」 | 五维保护原则（保留五官/肤色/骨相） |

---

## 🛠️ 怎么使用

### 1. 安装 (Claude Code)

将 `wsc-image` 文件夹放入你的技能目录：
```bash
~/.claude/skills/wsc-image/
```

### 2. 触发与交互
直接用口语描述你的想法。如果信息不够，AI 会自动弹出选择题引导你（风格 / 比例 / 节奏）。

### 3. 无限迭代
说「差一点」「再优化」可无限追问。AI 会弹出诊断菜单，精准调整你不满意的维度。

---

## 🗂️ 知识蒸馏工作流

你可以把你收集到的提示词技巧或风格参考（链接、文案、MD文件）发给 AI，并说：
> 「这是我收集的内容，请帮我提取核心规则并保存到技能记忆库中。」

AI 会自动将其压缩为结构化模式并存入 `memory/` 目录，使其成为技能的长期知识。

---

## 🎨 WSC Creative Suite 系列

- **[wsc-skill-image](https://github.com/weizhiyan/wsc-skill-image)** — AI 视觉创意专家（当前）
- **[wsc-skill-ux](https://github.com/weizhiyan/wsc-idea)** — UI/UX 设计与需求专家

---

> **Train your Skills like you train your models.**
> —— *WSC Creative Suite*
