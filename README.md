# 👤 Obsidian 个人数字档案（CRM）信息提取技能 (Obsidian CRM Extractor)

> 把简历、PDF、会议记录、新闻报道等非结构化文档，一键转成高密度、可量化、带双向链接的 Obsidian 联系人档案。

---

## 📌 背景与痛点

做商务、招聘、科研合作或投资人跟进时，人物信息散落在简历、访谈记录、会议纪要、新闻稿里：

1. **信息碎片化**：同一个人分散在多个文件，需要人工交叉比对。
2. **形容词代替事实**：全是“经验丰富”“极大提升”，没有数值、周期、产出。
3. **无法沉淀复用**：信息停留在临时聊天里，Obsidian 里没有可被双链检索的实体。
4. **格式不统一**：每次按心情写，日期、公司、职务字段各不相同。

**Obsidian CRM Extractor** 强制按统一 Markdown 模板输出：高信息密度 + 量化表格 + `[[双向链接]]` 实体 + 多级标签，可直接粘贴进 Obsidian。

---

## 🚀 核心特性

- **去形容词，只留事实**：剔除主观评价，提取数值、时间节点、项目周期、团队规模、预算、产出。
- **强制表格化**：工作经历、项目执行、核心指标一律表格呈现，不用纯文本堆砌。
- **Obsidian 原生语法**：公司 / 项目 / 术语 / 地名 / 人名全部 `[[双链]]`；标签形如 `#人物/高管/生命科学`。
- **D-T-P-R 决策视角**：把重大事件拆成 决策 / 任务 / 问题与风险三栏，便于回溯。
- **一键复制**：输出包裹在 Markdown 代码块中，可直接整段粘贴。

---

## 📦 安装

### Claude Code / Codex / OpenCode 等通用 Agent
把本仓库的 `SKILL.md` 放入你的 skills 目录：

```bash
git clone https://github.com/r4ain1/obsidian-crm-extractor.git
# 例如 Hermes：放到 <HERMES_HOME>/skills/<category>/obsidian-crm-extractor/
```

### Hermes Agent
```
skill_view(name='obsidian-crm-extractor')
```

---

## 🧭 使用方式

直接对 Agent 说：

> 把这份简历提取成 Obsidian 联系人档案。

或批量上传多个 PDF / 会议记录，Agent 会静默读取、交叉比对去重、按时间线重组后输出。

---

## 📄 输出结构

```
core profile      核心画像（定位 / 关键标签 / 联系方式）
metrics           核心数据与指标（量化能力表）
timeline          履历与项目执行（倒序表格）
network           实体关系网（汇报对象 / 团队 / 外部协作）
decisions         关键决策与事件（D-T-P-R）
attachments       附件与参考文献
```

---

## 📁 目录结构

```
SKILL.md      技能主文件（角色定义、处理原则、工作流、输出模板）
README.md     本文件
LICENSE       MIT
```

---

## 🔗 相关技能

- `obsidian-session-archive` — 会话与产物归档
- `weekly-plan-vs-actual` — 项目周报预实对比

---

## 📜 License

MIT © 2026 r4ain1
