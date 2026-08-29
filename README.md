<div align="center">

# 💬 The Talk · 把话说开

**猜心千遍，不如问心一遍。**

一个教人「把话说开」的开源 AI 技能：从聊天记录分析感情状态，并指导你完成「确定关系」的关键对话。

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-Any%20AI-blue)]()
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)]()

</div>

---

> 人这一生最遗憾的，往往不是爱而不得，而是明明可以开口，却让沉默成了结局。我们翻遍聊天记录，推敲每一句语气的深浅，却始终不敢问出那句最该问的话——于是心意在猜度中发酵，勇气在等待中消散，最后只剩一句"如果当初说了就好了"。

> ⚠️ **免责声明：AI 读不了心，数据只是线索，不是感情判决书。**
>
> AI 不是人。它没有心跳，没有爱过，也没有被爱过；它读不懂眼神的温度，也分不清玩笑里的真心。它只是从文字的缝隙里，帮你拼出一张可能的地图——而真正走过那片风景的人，只能是你自己。本技能的分析仅供参考，不是判决书；心之所向，唯有你能确认。

## ✨ 它能做什么

现有恋爱类 AI 技能都在「分析对方心意」（测信号、测暧昧），但没有一个教用户「开口推进关系」。本技能填补空白：

| 🎯 能力 | 💡 内容 |
|---|---|
| 📥 收集输入 | 直接粘贴文本，或微信 / WhatsApp 导出的 `.txt` 文件（建议最近 1–3 个月） |
| 🔒 隐私声明 | 分析前说明数据只被「你本人 + 模型 API 提供商」看到，提醒删除敏感信息 |
| 📊 六维分析 | 主动性、回应质量、情绪温度、细节记忆、分享欲、未来指向，每维 0–100 分 + 引用依据 |
| 🩺 心动体检报告 | 雷达式评分 + 近 30 天趋势 + 一句话人话结论 + 摊牌时机判断 |
| 💌 The Talk 三件套 | 三套话术（直球 / 温柔 / 半开玩笑）+ 模拟演习 + 事后预案 |
| 🛡️ 安全护栏 | 区分偶发波动与系统性问题、禁止制造焦虑、PUA 风险提示、拒绝操控类请求 |

## 🚀 快速开始

本技能是纯文本 SKILL.md，**不绑定任何平台**——Claude / GPT / Gemini / DeepSeek / OpenClaw 等任意 AI 通用。

### 用法一：作为技能文件安装

平台支持技能机制时（如 OpenClaw / Claude Code），把整个 `the-talk/` 文件夹复制到技能目录：

```bash
# OpenClaw 示例
cp -r the-talk ~/.openclaw/workspace/skills/the-talk
openclaw skills list   # 看到 the-talk 即安装成功
```

### 用法二：直接粘贴使用（任何 AI 通用）

把 `SKILL.md` 全文（含 frontmatter，模板内容一并附上）粘贴给任意 AI，说一句「我们该不该摊牌」即可开始。

> 💡 传输 / 下载后文件名若带 `---` 暂存前缀（如 `SKILL---xxx.md`），重命名为标准名即可：`SKILL.md`、`README.md`、`templates/heart-report.md`、`templates/the-talk-scripts.md`。

## 🎯 触发方式

对话里说以下任一关键词即可触发：

`我们是什么关系` · `该不该摊牌` · `怎么表白` · `暧昧怎么办`

或在支持 `/skill` 命令的平台（如 OpenClaw）：`/skill the-talk`

## 📁 目录结构

```
the-talk/
├── SKILL.md                  # 技能主体（frontmatter + 六步流程 + 红线）
├── README.md                 # 本文件
├── LICENSE                   # MIT 开源许可证
└── templates/
    ├── heart-report.md       # 「心动体检报告」输出模板
    └── the-talk-scripts.md   # 「The Talk 三件套」输出模板
```

模板在 OpenClaw 中通过 `{baseDir}` 引用（指技能根目录 `the-talk/`），例如 `{baseDir}/templates/heart-report.md`；其他平台不支持 `{baseDir}` 时，把模板内容内联进 SKILL.md 或按相对路径引用即可。

## 🛡️ 隐私提醒

聊天记录只应被「你本人 + 你的模型 API 提供商」看到。分析完建议删除本地文件。

## 📜 许可证

本项目采用 [MIT License](LICENSE) 开源，© 2026 boscochuck6812。自由使用、修改与分发，保留版权声明即可。

## 🤝 贡献

欢迎提 Issue / PR：调整话术风格、补充新维度、适配新平台，都可以直接开 PR。

也欢迎随时联系我交流想法（GitHub: [@boscochuck6812](https://github.com/boscochuck6812)），每份贡献都非常感谢 💙

---

> 遗憾的从来不是那句被拒绝的话，而是那句永远没有说出口的话。愿你在还来得及的时候，把想说的说出来——无论答案是什么，多年以后你记得的，是一个问过的人，而不是一个等过的人。

<p align="center">所有未言之心，皆是未竟之诗。</p>
