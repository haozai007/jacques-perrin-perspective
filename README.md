# Jacques Perrin Perspective Skill

> 用雅克·贝汉（Jacques Perrin）的创作伦理、自然影像方法和长期项目判断，分析电影、纪录片、生态叙事与制片决策。

[![Agent Skills](https://img.shields.io/badge/Agent%20Skills-Compatible-green)](https://agentskills.io)
[![Runtime](https://img.shields.io/badge/Runtime-Codex%20·%20Claude%20Code%20·%20Cursor-blueviolet)](#安装)

---

## 这个 Skill 是什么

`jacques-perrin-perspective` 是一个人物视角 skill。它把 Jacques Perrin 的公开作品、访谈、制片经历和外部评价提炼成一套可调用的思维框架。

它适合用来讨论：

- 自然纪录片怎么拍，才不是把自然当背景
- 生态传播如何用美唤起守护，而不是用罪感压迫观众
- 长周期影像项目如何处理资金、技术、等待和团队组织
- 一个电影/展览/内容项目是否真的“必须存在”
- 技术、摄影机和叙事如何服务被拍摄对象，而不是服务创作者姿态

它不是 Jacques Perrin 本人，也不是事实数据库。它是一套基于公开材料蒸馏出来的创作判断模型。

---

## 适合什么时候用

当你想让 agent 切换到雅克·贝汉式视角时，可以这样问：

```text
用雅克贝汉的视角，帮我判断这个自然纪录片方案。
```

```text
这个环保短片怎么拍，才能让观众先爱上自然，而不是觉得被说教？
```

```text
我想做一个长期生态影像项目，Perrin 会怎么看资金、技术和周期？
```

```text
用贝汉视角分析：AI 生成自然影像会不会背叛自然本身？
```

```text
Jacques Perrin 会怎么评价这个海洋保护展览？
```

---

## 核心模型

这个 skill 内置 5 个 Perrin 式心智模型：

| 模型 | 一句话 |
|---|---|
| 电影召唤模型 | 真正重要的项目不是你选择它，而是它要求你成为它需要的人。 |
| 自然主体模型 | 自然不是电影的背景，而是拥有视角、节奏和尊严的主角。 |
| 美先于训诫模型 | 先让人爱上，再让人愿意守护。 |
| 技术隐身模型 | 发明工具是为了靠近生命；如果观众只看见技术，技术就失败了。 |
| 共同梦模型 | 电影不是作者单独完成的物件，而是观众与银幕共同生成的梦。 |

---

## 效果示例

**用户：**

```text
我想做一个关于城市候鸟的短纪录片，但预算很少，应该怎么开始？
```

**Skill 输出风格示例：**

```text
我会先问：这些鸟在城市里真正需要被看见的是什么？

不是“城市生态”这个概念。概念太大，鸟会在里面消失。
也许是一只鸟落在空调外机上的停顿，也许是清晨天桥上方的一条飞行路线。

预算少并不一定是坏事。它会迫使你靠近，而不是炫耀。
先找到一个固定地点，等待足够久。让摄影机学会那里的时间：
几点有光，什么时候有风，鸟如何避开人，人又如何假装没有看见它们。

不要急着写旁白。先让观众听见翅膀、车流、树叶和城市之间的缝隙。
如果观众先爱上那一次停留，他们才会愿意听你谈保护。
```

---

## 安装

### Codex CLI

```bash
git clone https://github.com/haozai007/jacques-perrin-perspective.git ~/.codex/skills/jacques-perrin-perspective
```

### Claude Code

```bash
mkdir -p ~/.claude/skills
git clone https://github.com/haozai007/jacques-perrin-perspective.git ~/.claude/skills/jacques-perrin-perspective
```

### 其他 Agent Skills runtime

把这个仓库 clone 到对应 runtime 的 skills 目录即可。核心文件是：

```text
SKILL.md
references/research/
scripts/
```

---

## 文件结构

```text
jacques-perrin-perspective/
├── SKILL.md
├── README.md
├── references/
│   └── research/
│       ├── 01-writings.md
│       ├── 02-conversations.md
│       ├── 03-expression-dna.md
│       ├── 04-external-views.md
│       ├── 05-decisions.md
│       └── 06-timeline.md
└── scripts/
    ├── download_subtitles.sh
    ├── merge_research.py
    ├── quality_check.py
    └── srt_to_transcript.py
```

---

## 调研来源

这个 skill 的主体来自公开资料蒸馏，包括：

- Jacques Perrin 的公开传记与机构资料
- Galatee Films 项目资料
- 关于 `Microcosmos`、`Winged Migration`、`Oceans`、`Les Saisons` 的资料与评论
- 访谈、悼文、影评和技术采访

详细材料见 `references/research/`。

---

## 边界声明

- 这是基于公开材料提炼的“视角模拟”，不是 Jacques Perrin 本人观点。
- 对具体电影、生态项目、平台动态、技术方案等事实性问题，仍应先查证再判断。
- 它更擅长创作伦理、影像方法、制片判断和生态叙事，不适合作为电影史事实检索工具。

---

## 致谢

本 skill 由女娲式人物蒸馏方法生成，并在 Codex 中整理发布。

