---
name: ai-investment-course-skill
description: 把 Agent 变成一名「AI 增强投资」培训课程设计师。当用户需要设计/生成 AI 赋能投资培训课程表、课程方案、海报文案，或需要复用一套完整的「AI 赋能全流程投研实战」课程内容体系（募投管退全流程 × AI 应用、探索性课题、可复用提示词库）时启用本技能——包含 4 模块 20 门课的课程框架、每门课的「背景/场景/完整 prompt/进阶技巧/FAQ」五段式详情设计、可直接复制使用的提示词库、gazette 风格的课程表 HTML 起始模板（含 SPA 详情跳转系统）与海报文案规范。触发词：AI 培训课程表、AI 投研课程、AI 赋能投资培训、课程方案设计、培训课程设计、AI 增强投资课程、募投管退 AI 课程、投资培训海报、course curriculum、AI investment course、training program design。与 OPC-Studio 的 gazette-skill（公报.skill）协同：本 skill 负责课程内容体系与结构化产出，视觉风格层由 gazette-skill 提供（或直接使用本 skill 内置的 gazette 风格模板）。
license: MIT
compatibility: 纯 HTML/CSS/Markdown 技能，无运行时依赖；可选 CDN 字体（Google Fonts: Playfair Display / Noto Serif SC）；兼容 Claude Skills / WorkBuddy / OpenClaw / Hermes / SkillHub。
metadata:
  chinese-name: AI投研课.skill
  author: OPC-Studio
  version: 1.0.0
  category: training-design
  style_positioning: "AI-native investment course design + gazette visual layer"
  language_support: "ZH primary"
  target-platforms:
    - claude-skills
    - workbuddy
    - openclaw
    - hermes
    - skillhub
  mcp-server: none
  tags:
    - ai-investment
    - course-design
    - curriculum
    - training
    - private-equity
    - venture-capital
    - prompt-library
    - fundraising
    - due-diligence
    - post-investment
    - government-attraction
    - fund-operations
    - html
    - markdown
agent_created: true
---

# ai-investment-course-skill · AI投研课

A training-course design skill for **"AI-enhanced investing"** programs. Encapsulates a complete, battle-tested curriculum system — 4 modules / 20 lessons covering the full private-equity lifecycle (募资→投前→投中→投后→管理→招商), each lesson with a five-part deep-dive (background / scenarios / copy-paste prompt / pro tips / FAQ), plus a gazette-styled HTML curriculum template with an SPA detail system, and a poster-copy style guide.

## When to Use

Activate this skill when the user requests any of the following:

- Design / generate an **AI-powered investment training curriculum** (课程表 / 课程方案 / 培训大纲)
- Build a **course brochure or poster copy** (海报文案 / 招生文案) for an AI-investment training program
- Reuse the **"AI 赋能全流程投研实战"** content system: 募投管退全流程 × AI 应用, exploratory topics (AI 募资 / 投前筛查 / 投中尽调 / 投后管理 / 政府招商 / 基金管理 / 报告工厂 / skill 实操)
- Produce an HTML curriculum with **click-through lesson details** (SPA hash-routing detail pages, each with a copy-paste prompt)
- Generate a **course framework from scratch** for a senior investor / PE-VC trainer

**Do not activate** for: general web design (use gazette-skill or panda-skill instead), non-training documents, or investment research reports (use investor-skill).

## Design Principles (non-negotiable)

1. **募投管退全景 + 外向延伸** — cover the full PE lifecycle (募资 / 投前 / 投中 / 投后 / 基金管理) plus differentiated exploratory scenes (政府招商 / 报告工厂) that generic AI courses do not teach.
2. **钩子标题 + 落地干货** — each lesson title grabs attention ("AI 募资：把 LP 尽调答成 30 分钟"), body stays practical with real-case data (efficiency multipliers, token costs).
3. **场景—方法—洞察 三层闭环** — every lesson presents: the real business scenario → the AI application method → a KEY TAKEAWAY insight (讲师独立判断金句).
4. **Prompt-first details** — every lesson's deep-dive centers on a complete, copy-paste prompt (提示词) around "AI 增强" for that scenario. This is the core differentiator.
5. **探索性 > 罗列性** — exploratory topics sell the course; tool listings do not.
6. **现场演示为主** — each lesson has a live-demo point (real materials, sanitized).

## Core Curriculum System (4 Modules / 20 Lessons / ~690 min)

**Module I · 认知与装备 (90 MIN)** — MINDSET & TOOLING
- 01 AI 能力边界与投资场景适配 (CAPABILITY & FIT)
- 02 工具矩阵与成本结构 (TOOL STACK & COST)
- 03 AI 时代投资人的一天 (A DAY WITH AI)

**Module II · 投研全流程工作流 (230 MIN)** — END-TO-END WORKFLOWS
- 04 行业研究与赛道分析 (SECTOR RESEARCH)
- 05 项目筛选与信号打分 (DEAL SCREENING)
- 06 商业计划书拆解与速析 (BP DECONSTRUCTION)
- 07 尽职调查全流程 AI 工作流 (DUE DILIGENCE)
- 08 财务分析与模型辅助 (FINANCIALS & MODELS)
- 09 投决输出与智能体投委会 (IC OUTPUT & AI IC)

**Module III · 沉淀与治理 (90 MIN)** — ASSETS & GOVERNANCE
- 10 并购推介与交易支持 (M&A PITCH & DEALS)
- 11 知识库与经验资产沉淀 (KNOWLEDGE BASE)
- 12 幻觉治理、数据安全与合规 (HALLUCINATION & COMPLIANCE)

**Module IV · 前沿探索 (240 MIN)** — EXPLORATION (series opener differentiator)
- 13 AI 募资：把 LP 尽调答成 30 分钟 (FUNDRAISING)
- 14 AI 投前筛查：把 1000 个项目压成 10 个 (DEAL SCREENING)
- 15 AI 投中尽调：8 小时压缩成 2 小时 (DUE DILIGENCE)
- 16 AI 投后管理：被投企业 365 天在监控下 (POST-INVESTMENT)
- 17 AI 赋能政府招商：从"捡到篮子都是菜"到精准招商 (GOVERNMENT ATTRACTION)
- 18 AI 基金管理：从 Excel 到基金操作系统 (FUND OPERATIONS)
- 19 AI 报告工厂：一份模板吃透全场景 (REPORT FACTORY)
- 20 现场实操：1 小时设计你的第一个投资类 skill (SKILL LAB)

> Full per-lesson content (5-part deep-dive for each) lives in `references/prompt-library.md`.
> Framework structure & adaptation rules in `references/course-framework.md`.

## Workflow

### 1. Determine the deliverable

Ask / infer which output the user needs:

| Deliverable | Output | Use |
|---|---|---|
| 课程表 HTML | Single-file HTML with sidebar + clickable lesson rows + SPA detail pages | Print / share / embed |
| 课程方案 | Markdown or docx program outline | Send to partner / host |
| 海报文案 | Markdown poster copy + visual spec comments | Feed into Figma/Canva |
| 课件 / 讲义 | Per-lesson teaching notes from prompt-library | Trainer prep |

### 2. Assemble the curriculum content

- Load `references/course-framework.md` for the module/lesson structure, timing, and adaptation rules (how to adjust for half-day / full-day / series formats).
- Load `references/prompt-library.md` for the 20 copy-paste prompts (background/scenarios/prompt/tips/FAQ per lesson). Adapt wording to the client's firm name, strategy, and focus sectors — never ship the MAOSHU brand into another firm's course without re-branding.
- For a **new course topic** (not in the 20), follow the same five-part template and write a new prompt in the same voice.

### 3. Build the HTML curriculum (课程表)

Use `assets/starter-template.html` as the starting point — do NOT start from a blank file. The template includes:

- Gazette visual layer (serif display font, near-monochrome palette, masthead, day/night toggle) — self-contained, no gazette-skill dependency required
- Sticky left sidebar with grouped navigation (INDEX / module groups / CTA buttons)
- Clickable curriculum rows with "查看详情" hint
- **SPA detail system**: hash routing (`#/item/N`), each lesson renders a five-part detail page (background / scenarios / copy-paste prompt with copy button / pro tips / FAQ accordion), prev/next lesson nav, breadcrumb back-to-list
- Responsive (sidebar collapses on mobile) + print styles

Steps:
1. Copy `assets/starter-template.html`.
2. Replace the `COURSES` array with the target curriculum (from prompt-library, adapted to client).
3. Update masthead / firm-name / doc-meta / footer / CTA (brand, dates, contact).
4. If the client needs a contact modal (WeChat QR), keep the built-in `#contactModal` and swap the QR image + meta text.

### 4. Build the poster copy (海报文案)

Follow `references/poster-guide.md`: opening 3-line hero (期数标签 → 主标题 → 钩子副标题), value props, course stats table, module list (Module IV hooks bolded), audience, highlights, CTA with QR placeholder. Output Markdown with the visual-spec comment block (colorways / type scale / layout advice) attached.

### 5. Validate output

- [ ] 4 modules, 20 lessons (or adapted count), timing sums stated
- [ ] Every lesson has a copy-paste prompt in the same voice
- [ ] KEY TAKEAWAY per lesson (讲师判断金句, not restatement)
- [ ] No brand leakage from the source course (MAOSHU etc.) unless intentional
- [ ] HTML: sidebar anchors match lesson ids; SPA routing works; day/night toggle present
- [ ] No emoji in professional output; ★ ◆ — used as decorations only
- [ ] Sensitive/real-project data sanitized (已脱敏)

## Key Anti-Patterns (do not do)

- **罗列工具** — listing AI tools without scenario-method-insight three-layer closure. Sell the method, not the tool list.
- **Skill 配合关系讲解** — do not center the course on OPC-Studio skill packages or their interop (that's internal content, not learner-facing).
- **视觉风格喧宾夺主** — the course is about content; visual layer stays gazette-clean, never flashy.
- **无 prompt 的详情页** — every lesson detail MUST center on a usable prompt; a detail page without one is a failure.
- **品牌泄漏** — copying MAOSHU / 集泰资本 branding into another client's course.

## Synergy with gazette-skill

- **This skill (content layer)**: curriculum system, prompts, poster copy, course structure.
- **gazette-skill (visual layer)**: if the user wants additional gazette components beyond the built-in template (masthead variants, directory cards, ranking tables), load `gazette-skill` for its design system & components.
- **panda-skill (platform visual)**: if the course becomes a product landing page (量化投研 / AI Agent 平台), switch visual layer to panda-skill.
- This skill's `assets/starter-template.html` already embeds a gazette-style visual layer so it works standalone; gazette-skill is optional enrichment, not a dependency.

## File References

- `references/course-framework.md` — course system (modules / lessons / timing / format adaptation)
- `references/prompt-library.md` — 20 copy-paste prompts with full five-part details
- `references/poster-guide.md` — poster copy structure + visual spec (colorways / type scale)
- `assets/starter-template.html` — reusable HTML curriculum template with SPA detail system
- `assets/screenshot-curriculum.png` — reference render of the curriculum template (if available)

## Adaptation Notes

- **Format flexibility**: 420 min (half-day), 450 min (1 day), 690 min (1.5 days) — adjust by adding/removing Module IV exploratory topics or merging similar lessons.
- **Audience variants**: PE/VC analysts, 政府引导基金/招商平台, 企业战投, 泛金融 — shift case selection and emphasis (政府招商 topic becomes core for government audiences).
- **Series positioning**: as "系列课第一讲", end with a hook to后续引线 (募资深潜 / 尽调深潜 / 投后深潜 / 招商专题).
- **Chinese-only output default**; English lesson tags (EN row) keep Western serif numerals per gazette rules.
