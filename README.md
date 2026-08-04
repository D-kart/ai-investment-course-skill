# AI投研课.skill · ai-investment-course-skill

> 把 Agent 变成一名「AI 增强投资」培训课程设计师。

---

## 这是什么

`ai-investment-course-skill` 是一个符合 [agentskills.io](https://agentskills.io) 开放规范的 AI Agent 技能包。
安装后，你的 Agent 将具备 **「AI 赋能全流程投研实战」课程体系** 的完整设计与产出能力——
从课程框架、每门课的五段式深度内容（含可复制提示词）、到 gazette 风格的课程表 HTML（含 SPA 详情系统）与招生海报文案。

与 OPC-Studio 的 [gazette-skill](https://github.com/D-kart/gazette-skill) 协同：
本 skill 是**内容层**（课程体系 + prompt 库 + 产出结构），gazette-skill 是**视觉层**（如需更多公报风格组件可加载）。

---

## 它能做什么

| # | 能力 | 产出 |
|---|---|---|
| 1 | **课程框架设计** | 4 模块 / 20 门课 / 690 分钟「募投管退全流程 × AI 应用」体系（可适配半日/全日/系列课） |
| 2 | **五段式课程详情** | 每门课：背景说明 / 适用场景 / 完整可复制 prompt / 进阶技巧 / FAQ |
| 3 | **提示词库** | 20 条围绕「AI 增强投资」场景的可复用 prompt（DDQ 应答 / 产业地图 / BP 拆解 / 纪要官 / 智能体投委会 / 招商地图 / LP 报告…） |
| 4 | **课程表 HTML** | gazette 风格单文件模板，含 sticky sidebar + 点击进详情（SPA hash 路由）+ 复制按钮 + 昼夜切换 |
| 5 | **招生海报文案** | Markdown 海报文案 + 视觉规范（深墨金/黑金双配色、字号层级、排版建议） |
| 6 | **再品牌化** | 一键替换占位符适配任意机构/讲师，杜绝源课程品牌泄漏 |

---

## 何时触发

> AI 培训课程表、AI 投研课程、AI 赋能投资培训、课程方案设计、培训课程设计、AI 增强投资课程、募投管退 AI 课程、投资培训海报、course curriculum、AI investment course、training program design……

---

## 核心输出风格

- 🎓 **募投管退全景 + 外向延伸**：募资 / 投前 / 投中 / 投后 / 基金管理 + 差异化探索课题（政府招商 / 报告工厂）
- 🪝 **钩子标题 + 落地干货**：「AI 募资：把 LP 尽调答成 30 分钟」「把 1000 个项目压成 10 个」
- 📝 **Prompt-first**：每门课详情以一条可直接复制的提示词为核心，围绕「AI 增强」场景设计
- 💡 **KEY TAKEAWAY 金句**：每课一条讲师独立判断（「对手不是隔壁城市，是信息差」）
- 📰 **gazette 视觉层**：衬线大标题 + 黑白单色 + 报头元素 + 昼夜切换（模板自带，无需额外依赖）

---

## 快速上手

### 在 Claude / WorkBuddy 中使用

1. 下载 `ai-investment-course-skill/` 文件夹，放入 `~/.claude/skills/` 或 `~/.workbuddy/skills/`。
2. 重启客户端，向 Agent 说：**"帮我设计一个 AI 赋能投资培训课程表"** 或 **"用这套课程体系生成海报文案"**，技能自动触发。

### 在 OpenClaw / Hermes 中使用

1. 将 `ai-investment-course-skill/` 放入 `skills/` 目录。
2. 通过 `skill_view` 查看 SKILL.md 加载。

### 在 SkillHub 中使用

1. 打包：`zip -r ai-investment-course-skill.zip ai-investment-course-skill/`
2. 登录 SkillHub，点击"上传 Skill"，选择 zip 文件。

---

## 目录结构（三层架构）

```
ai-investment-course-skill/
├── SKILL.md                          # 主路由（必读）
├── CHANGELOG.md                      # 版本日志
├── README.md                         # GitHub 门面
├── LICENSE                           # MIT
├── references/                       # 📚 REFERENCES 具体规范
│   ├── course-framework.md           # 课程体系框架（模块/课时/适配规则/再品牌化）
│   ├── prompt-library.md             # 20 条可复用提示词库（五段式详情）
│   └── poster-guide.md               # 海报文案规范（结构/配色/字号/排版）
└── assets/                           # 🅰️ ASSETS 资产真源
    └── starter-template.html         # 课程表 HTML 起始模板（含 SPA 详情系统）
```

> 三层架构：**META**（SKILL.md frontmatter）· **ASSETS**（assets/ 资产真源）· **REFERENCES**（references/ 具体规范）。

---

## 与 OPC-Studio 其他 skill 协同

- **内容层**：`ai-investment-course-skill`（课程设计）· [investor-skill](https://github.com/D-kart/investor-skill)（投资工作流）
- **视觉层**：[gazette-skill](https://github.com/D-kart/gazette-skill)（报告/课程表·古典公报风）· [panda-skill](https://github.com/D-kart/panda-skill)（平台落地页·双色 SaaS 风）
- 本 skill 的课程表模板已内嵌 gazette 视觉层，可独立工作；需要额外公报组件时加载 gazette-skill。

---

## 许可证

MIT License · © 2026 OPC-Studio

---

## 反馈与贡献

- Issue / PR：欢迎在本仓库提交
- 兼容问题：请附上平台名与 Agent 版本号
- 内容扩展：期待更多场景课程（二级市场 AI 投研、跨境并购、S 基金等）的贡献

---

_OPC-Studio 出品 · 让每个 AI Agent 都能成为行业专家。_
