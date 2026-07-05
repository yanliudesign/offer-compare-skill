# Offer Compare Skill

> 拿到两份（或多份）offer 纠结怎么选？把它扔给一个**有立场、会得罪人**的 Senior Career Decision Advisor，一份 HTML 决策报告就出来了。

---

## 3 步

1. **贴两份 offer**
   Offer A / Offer B — Company / Role / Level / Location / TC breakdown（Base + Bonus + RSU + Sign-on）
2. **补 priorities & 当前处境**（optional 但强烈建议）
   钱 / 成长 / AI / 稳定 / 生活方式 / visa / burnout / deadline ...
3. **自动生成 HTML Decision Report**
   写到 `~/Desktop/Claude skills/offer-compare-<A>-vs-<B>-<YYYYMM>.html` 并自动在浏览器打开。

---

## 报告里有什么

- **Verdict** — 一条明确推荐（不允许中性）+ ⭐ 决心指数
- **Assumptions** — 显式列出所有假设（RSU vest / 币种汇率 / bonus target / 股价波动），任一不对可以让 skill 重跑
- **§1 · Offer Breakdown** — Base / Bonus / RSU / Sign-on / 4-year TC 区间 / equity risk / stability，表格对照
- **§2 · Dimension Compare** — 7 维评分：💰 Comp · 📈 Growth · 🤖 AI Exposure · 🏢 Company Strength · 👤 Manager/Team Risk · 🔁 Promo Speed · 🌍 Lifestyle
- **§3 · Hidden Signals** — 5 条隐藏信号：front-loaded · long-term upside · uncertainty · resume value · switch-out difficulty
- **§4 · Risk Analysis** — 每份 offer 4-6 条 risk（equity / role / team / market / life）
- **§5 · Recommendation** — 明确推荐 + tradeoff + "If you are X → A / If you are Y → B" 分叉判定

+ EN / 中文 双语切换 · Export PDF · Export Markdown

---

## 三条铁律

1. **不许中性。** 必须给一条明确推荐，同时用 "If X → A / If Y → B" 兜底另一类人。
2. **数字给区间 + 显式假设。** 4 年 TC 永远给 `$X ~ $Y`，不给单点。所有假设在顶部 Assumptions 显式列出。
3. **不编事实。** 用户没说过的数字标 `[需用户补充]`；公司信号只能从公开信息 + 用户提供推断，标"我从 ___ 推断"。

---

## 结构

```
offer-compare-skill/
├── SKILL.md                              ← 主入口
├── README.md                             ← 你正在读这个
├── prompts/                              ← 5 条内部流程
│   ├── offer-breakdown.md
│   ├── dimension-compare.md
│   ├── hidden-signals.md
│   ├── risk-analysis.md
│   └── recommendation.md
├── frameworks/                           ← 评分标准 + 报告规格
│   ├── dimension-rubric.md
│   ├── hidden-signals-dictionary.md
│   ├── risk-taxonomy.md
│   └── offer-compare-report.md          ← HTML 报告规格（最重要）
├── examples/
│   └── offer-compare-template.html      ← 视觉骨架
└── offer-bank/                          ← 历史决策库
    ├── _index.md
    └── _template.md
```

---

## 位置

跟 `job-description-skill/` / `resume-skill/` / `bq-skill/` 一起放进 `offer-toolkit-skill/` 或 `~/.claude/skills/`，也可以单独装。

---

Created by [Dreameryanyan](https://www.linkedin.com/in/yanliudesign/) · [LinkedIn](https://www.linkedin.com/in/yanliudesign/) · [X](https://x.com/yanliudreamer) · [小红书](https://www.xiaohongshu.com/user/profile/5b2afdf311be104ac3c22931)
