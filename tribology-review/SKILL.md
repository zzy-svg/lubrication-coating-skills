---
name: tribology-review
description: >
  Write comprehensive literature reviews for lubrication coating materials and tribology research.
  Use when writing survey papers, systematic reviews, or literature analyses on topics like solid lubricants,
  DLC coatings, MoS2, WS2, self-lubricating coatings, wear-resistant coatings, or tribological applications.
  Triggers on requests for "review paper", "survey", "literature review", "综述", "tribology review",
  "coating review", or mentions of lubrication coatings, friction, or wear research.
metadata:
  author: user
  version: "1.0.0"
allowed-tools:
  - Read
  - Write
  - Edit
  - Glob
  - Grep
  - Bash
  - WebSearch
  - WebFetch
  - Task
  - mcp__arxiv-mcp-server__search_papers
  - mcp__arxiv-mcp-server__download_paper
  - mcp__arxiv-mcp-server__read_paper
  - mcp__scholar-mcp-server__search
  - mcp__scholar-mcp-server__get_paper_details
  - mcp__scholar-mcp-server__get_citations
  - mcp__zotero__zotero_search_items
  - mcp__zotero__zotero_get_item_fulltext
  - mcp__zotero__zotero_create_item
  - mcp__pubmed__pubmed_search_articles
  - mcp__pubmed__pubmed_get_article_details
  - mcp__pubmed__pubmed_get_fulltext
---

# Tribology Coating Literature Review Skill

## 润滑涂层材料文献综述撰写技能

---

## Quick Start | 快速开始

1. **Initialize project** with three core files:
   - `CLAUDE.md` - Writing guidelines and terminology
   - `IMPLEMENTATION_PLAN.md` - Staged execution plan
   - `manuscript_draft.md` - Main manuscript

2. **Follow the 7-phase workflow** (see [references/WORKFLOW.md](references/WORKFLOW.md))

3. **Use domain-specific templates** (see [references/DOMAINS.md](references/DOMAINS.md))

---

## Core Principles | 核心原则

### Writing Style | 写作风格

- **Hedging language**: "may", "suggests", "appears to", "has demonstrated", "indicate that"
- **避免绝对表述 | Avoid absolutes**: Never say "X is the best coating"
- **引用支持 | Citation support**: Every technical claim needs reference
- **定量数据 | Quantitative data**: Always include specific metrics (COF, wear rate, hardness)

### Required Elements | 必需元素

- **Key Points box** (3-5 bullets) after title | 标题后关键发现摘要（3-5点）
- **Comparison tables** for each coating category | 每类涂层的对比表格
- **Performance metrics**: COF (0.0X-0.X), Wear rate (10^-X mm³/Nm) | 性能指标
- **Figure placeholders** with detailed captions (SEM, TEM, Raman, etc.) | 图表占位符
- **References**: 80-120 typical, organized by topic | 参考文献（80-120篇，按主题分类）

### Coating Description Template | 涂层描述模板

```markdown
### 3.X [Coating Category]

**[Coating Name]:** [Author] et al. [year] developed [coating], which features:
- [Key composition/structure 1]
- [Key composition/structure 2]

Achieved COF of 0.XX and wear rate of X×10^-X mm³/Nm on [substrate].

**Limitations:** Despite advantages, [category] coatings face:
(1) [limitation 1 - e.g., oxidation at high temperature]
(2) [limitation 2 - e.g., poor adhesion to certain substrates]
```

---

## Literature Sources | 文献来源

| Source | Best For | 用途 | Tools |
|--------|----------|------|-------|
| ArXiv | Latest materials synthesis, ML in tribology | 最新材料合成、摩擦学机器学习 | `search_papers`, `read_paper` |
| Google Scholar | Broad coverage, citation tracking | 广泛覆盖、引文追踪 | `scholar-mcp-server` |
| PubMed | Biomedical, clinical research | 生物医学、临床研究 | `pubmed_search_articles` |
| Zotero | Personal library, reference management | 个人文献库、参考文献管理 | `zotero_search_items` |
| Web of Science | High-quality journal articles | 高质量期刊文章 | WebSearch |
| Specific Journals | Tribology International, Wear, Coatings | 专业期刊直接搜索 | Direct journal search |

**See | 参见**: [references/LITERATURE_SOURCES.md](references/LITERATURE_SOURCES.md)

---

## Standard Review Structure | 标准综述结构

```markdown
# [Title]: State of the Art and Future Directions in [Coating Type] Coatings
## [副标题: 最新进展与未来展望]

## Key Points | 关键发现
- [3-5 bullets summarizing main findings | 总结主要发现的3-5个要点]

## Abstract | 摘要

## 1. Introduction | 引言
### 1.1 Tribological Background and Significance | 摩擦学背景与意义
### 1.2 Lubrication Mechanisms | 润滑机制
### 1.3 Scope and Contributions | 研究范围与贡献

## 2. Coating Classification and Materials | 涂层分类与材料
### 2.1 Solid Lubricant Coatings | 固体润滑涂层 (MoS2, WS2, h-BN, Graphite)
### 2.2 Diamond-Like Carbon (DLC) Coatings | 类金刚石涂层
### 2.3 Metal-Based Self-Lubricating Coatings | 金属基自润滑涂层
### 2.4 Ceramic Coatings | 陶瓷涂层 (TiN, CrN, Al2O3)
### 2.5 Multilayer/Composite Coatings | 多层/复合涂层

## 3. Deposition Techniques | 沉积技术
### 3.1 Physical Vapor Deposition (PVD) | 物理气相沉积
### 3.2 Chemical Vapor Deposition (CVD) | 化学气相沉积
### 3.3 Thermal Spray Methods | 热喷涂方法
### 3.4 Electroplating and Electroless Plating | 电镀与化学镀

## 4. Characterization Methods | 表征方法
### 4.1 Mechanical Properties | 机械性能 (Hardness, Adhesion)
### 4.2 Surface Characterization | 表面表征 (SEM, AFM, XPS)
### 4.3 Structural Analysis | 结构分析 (XRD, Raman)

## 5. Tribological Performance | 摩擦学性能
### 5.1 Friction Coefficients | 摩擦系数 (Table 2)
### 5.2 Wear Rates and Mechanisms | 磨损率与机制
### 5.3 Environmental Effects | 环境影响 (Temperature, Humidity)

## 6. Applications | 应用
### 6.1 Aerospace Components | 航空航天部件
### 6.2 Automotive Parts | 汽车零部件
### 6.3 Biomedical Implants | 生物医疗植入物
### 6.4 Cutting Tools and Molds | 切削工具与模具

## 7. Challenges and Future Directions | 挑战与未来方向

## 8. Conclusion | 结论

## References | 参考文献
```

---

## Key Metrics Reference | 关键指标参考

| Metric | Symbol | Typical Range | Unit | 说明 |
|--------|--------|---------------|------|------|
| Coefficient of Friction | COF | 0.01 - 0.8 | - | 摩擦系数 |
| Wear Rate | WR | 10^-8 - 10^-3 | mm³/Nm | 磨损率 |
| Hardness | H | 1 - 80 | GPa | 硬度 |
| Elastic Modulus | E | 100 - 1000 | GPa | 弹性模量 |
| H/E Ratio | H/E | 0.05 - 0.15 | - | 硬弹比 |
| Adhesion Strength | Lc | 5 - 100 | N | 附着力 |

**See | 参见**: [references/METRICS.md](references/METRICS.md)

---

## Citation Patterns | 引用模式

```markdown
# 性能数据引用 | Performance data citation
"...achieved COF of 0.08 [23]"

# 方法引用 | Method citation
"Li et al. [45] developed..."

# 比较引用 | Comparative citation12] focused on
"While [ DLC coatings, [15] addressed MoS2-based..."

# 多引用 | Multi-citation
"Several studies demonstrated... [12, 15, 23]"
```

---

## Reference Files | 参考文件

| File | Purpose | 用途 |
|------|---------|------|
| [references/WORKFLOW.md](references/WORKFLOW.md) | Detailed 7-phase workflow | 详细七阶段工作流 |
| [references/DOMAINS.md](references/DOMAINS.md) | Coating categories and methods | 涂层分类与方法 |
| [references/METRICS.md](references/METRICS.md) | Tribological metrics and standards | 摩擦学指标与标准 |
| [references/LITERATURE_SOURCES.md](references/LITERATURE_SOURCES.md) | Journal and database guide | 期刊与数据库指南 |
| [references/TEMPLATES.md](references/TEMPLATES.md) | Project templates | 项目模板 |
| [references/QUALITY_CHECKLIST.md](references/QUALITY_CHECKLIST.md) | Pre-submission checklist | 投稿前检查清单 |
| [references/MCP_SETUP.md](references/MCP_SETUP.md) | MCP server configuration | MCP服务器配置 |

---

## Usage Examples | 使用示例

### Example 1 | 示例1

**User | 用户**:
```
/tribology-review
我想写一篇关于"DLC涂层在高温环境下摩擦学性能"的文献综述，
重点关注DLC涂层的氧化行为和摩擦稳定性。
```

**System Response | 系统响应**:
1. Create project structure (CLAUDE.md, IMPLEMENTATION_PLAN.md, manuscript_draft.md)
2. Search ArXiv for latest DLC high-temperature research
3. Search Google Scholar for DLC oxidation studies
4. Generate detailed outline with sections on:
   - DLC types and their thermal stability
   - Oxidation mechanisms at high temperature
   - Doping strategies for improved thermal stability
   - Comparative performance data

### Example 2 | 示例2

**User | 用户**:
```
tribology review
Survey paper on solid lubricant coatings (MoS2, WS2, h-BN)
for aerospace applications
```

**System Response | 系统响应**:
1. Initialize review project
2. Collect literature from ArXiv, Google Scholar, Web of Science
3. Create literature matrix by coating type
4. Generate outline covering:
   - Introduction to solid lubricants
   - Coating deposition methods
   - Tribological performance comparison
   - Aerospace application requirements
   - Future research directions

---

## Language Support | 语言支持

This skill supports both English and Chinese content generation:

| Component | English | Chinese |
|-----------|---------|---------|
| Section Headers | English | Chinese (Bilingual headers) |
| Body Text | English preferred | Chinese supported |
| Citations | Standard format | GB/T 7714 supported |
| Terminology | Standard terms | 标准术语对照表 |

---

## Best Practices | 最佳实践

1. **Start with clear research scope**: Define coating type, application, and time period
   | 明确研究范围：定义涂层类型、应用领域和时间范围

2. **Use multiple literature sources**: Combine ArXiv (latest), Google Scholar (broad), and journals (high-quality)
   | 使用多源文献：ArXiv（最新）、Google Scholar（广泛）、期刊（高质量）

3. **Include quantitative data**: Always report specific COF, wear rate, and hardness values
   | 包含定量数据：始终报告具体的COF、磨损率和硬度值

4. **Structure for readability**: Use tables for comparison, figures for mechanisms
   | 结构清晰易读：使用表格对比、图表展示机制

5. **Follow consistency**: Maintain consistent terminology and citation format throughout
   | 保持一致性：全文术语和引用格式统一

---

## Troubleshooting | 常见问题

### Q: How to find the most relevant papers?
**A**: Use specific keywords and combine multiple sources. Start with broad search using keywords like "DLC coating friction coefficient", then narrow down by reading abstracts.

### Q: What if I cannot access certain journals?
**A**: Use ArXiv for preprints, Google Scholar for available versions, and request through interlibrary loan if necessary.

### Q: How many references should I include?
**A**: Typical reviews include 80-120 references. Focus on quality and relevance over quantity.

### Q: 如何找到最相关的论文？
**A**: 使用具体关键词并结合多个数据库。从"DLC涂层摩擦系数"等关键词的广泛搜索开始，然后通过阅读摘要缩小范围。

### Q: 如果无法访问某些期刊怎么办？
**A**: 使用ArXiv获取预印本，Google Scholar获取可用版本，必要时通过馆际互借获取。

### Q: 应该包含多少篇参考文献？
**A**: 典型综述包含80-120篇参考文献。注重质量和相关性而非数量。

---

**For detailed workflow | 详细工作流参见**: [references/WORKFLOW.md](references/WORKFLOW.md)
