# Literature Workflow | 文献收集工作流

This document provides systematic guidance on literature collection for tribology and coating research proposals.

本文档为摩擦学和涂层研究计划提供系统的文献收集指导。

---

## 1. Literature Collection Strategy | 文献收集策略

### Phase 1: Broad Survey | 阶段1：广泛调研

#### 1.1 Initial Search | 初始搜索

**Purpose**: Identify major works and themes

**Sources | 来源**:
| Source | Tool | Coverage |
|--------|------|----------|
| Google Scholar | WebSearch | Broad academic |
| ArXiv | search_papers | Latest preprints |
| Reviews | Google Scholar | Comprehensive |

**Search Strategy | 搜索策略**:
```markdown
# Broad queries
"tribology coating review"
"lubrication coatings review"
"DLC coating comprehensive review"
"solid lubricant review"
```

**Identify | 识别**:
- Key review papers (10+ citations)
- Foundational works (often review articles)
- Major research groups

#### 1.2 Key Paper Collection | 关键论文收集

**Collect | 收集**:
| Paper Type | Count | Purpose |
|------------|-------|---------|
| Review papers | 5-10 | Overview, gaps |
| Foundational | 5-10 | Background |
| Recent advances | 15-20 | State-of-the-art |
| Methods | 10-15 | Methodology |

### Phase 2: Focused Search | 阶段2：定向搜索

#### 2.1 Topic-Specific Search | 主题定向搜索

**By Method | 按方法**:
| Method | Keywords |
|--------|----------|
| PVD | "magnetron sputtering DLC" |
| CVD | "PECVD diamond-like carbon" |
| ML | "machine learning coating optimization" |

**By Property | 按性能**:
| Property | Keywords |
|----------|----------|
| Friction | "DLC coefficient of friction temperature" |
| Wear | "DLC wear rate mechanisms" |
| Temperature | "self-lubricating high temperature" |

#### 2.2 Citation Tracking | 引文追踪

**Backward | 向后**:
- Check references of key papers
- Look for seminal works

**Forward | 向前**:
- "Cited by" feature on Google Scholar
- Recent citations indicate impact

**Related Papers | 相关论文**:
- "Related articles" suggestions
- Same journal/author follow-up

---

## 2. Source Prioritization | 来源优先级

### 2.1 By Source Type | 按来源类型

| Priority | Source | Use When |
|----------|--------|----------|
| 1 | Review papers | Overview, gaps |
| 2 | Q1/Q1 journals | High-quality data |
| 3 | Q2 journals | Supporting data |
| 4 | ArXiv preprints | Latest methods |
| 5 | Conference papers | Recent advances |

### 2.2 By Recency | 按时效性

| Time Period | Weight | Purpose |
|-------------|--------|---------|
| 2019-2024 | 60% | Current state |
| 2014-2018 | 25% | Development history |
| Before 2014 | 15% | Foundational |

---

## 3. Literature Matrix | 文献矩阵

### 3.1 Template | 模板

| Category | Authors | Year | Title | Journal | Key Finding | COF/Wear | Reference |
|----------|---------|------|-------|---------|-------------|----------|-----------|
| DLC | Zhang 2023 | "DLC high temp" | Tribol. Int. | COF<0.1@400°C | 0.08 | [1] |
| MoS₂ | Liu 2022 | "MoS₂ review" | Surf. Coat. | Comprehensive | - | [2] |
| ML | Wang 2023 | "ML coating" | Appl. Surf. Sci. | ML prediction | - | [3] |

### 3.2 Data Extraction | 数据提取

| Property | Where to Find | Format |
|----------|---------------|--------|
| COF | Results section | 0.XX ± 0.XX |
| Wear rate | Results section | X×10^-X mm³/Nm |
| Hardness | Methods/Results | XX GPa |
| Temperature | Throughout | XX °C |
| Method | Methods | Deposition type |
| Substrate | Methods | Material |

---

## 4. Topic-Specific Literature | 主题特定文献

### 4.1 DLC Coatings | DLC涂层

| Topic | Key Papers | Focus |
|-------|------------|-------|
| Fundamentals | [1-5] | Structure, properties |
| Deposition | [6-10] | PVD, CVD methods |
| Doping | [11-15] | Si, N, metal doping |
| Temperature | [16-20] | High-temp stability |
| ML/AI | [21-25] | Prediction, optimization |

### 4.2 Solid Lubricants | 固体润滑剂

| Topic | Key Papers | Focus |
|-------|------------|-------|
| MoS₂ | [26-30] | Basal plane lubrication |
| WS₂ | [31-33] | High-temp stability |
| h-BN | [34-36] | Thermal stability |
| Composites | [37-40] | Synergistic effects |

### 4.3 Methods | 方法

| Method | Key Papers | Focus |
|--------|------------|-------|
| Sputtering | [41-45] | Parameter optimization |
| PECVD | [46-50] | Process control |
| Characterization | [51-55] | Testing standards |
| ML | [56-60] | Data-driven design |

---

## 5. Gap Identification | 空白识别

### 5.1 Types of Gaps | 空白类型

| Gap | Description | Literature Search |
|-----|-------------|-------------------|
| Knowledge | Missing understanding | Compare claims across papers |
| Method | No suitable approach | Review methods sections |
| Data | No quantitative data | Extract numbers |
| Application | No application | Check application sections |

### 5.2 Gap Analysis | 空白分析

**Template | 模板**:
```markdown
## Identified Gaps

### Gap 1: [Topic]
**Current State**: [What is known]
**Missing**: [What is not known]
**Evidence**: [Reference supporting gap]
**Opportunity**: [How your research addresses]
```

**Example | 示例**:
```markdown
### Gap 1: DLC stability above 500°C
**Current State**: DLC coatings show good tribological properties
up to 400°C, with COF increase at higher temperatures [1, 2].

**Missing**: Understanding of oxidation mechanisms and
stabilization strategies above 500°C [3].

**Evidence**: Only 3 papers address 500-800°C range,
all preliminary studies [3-5].

**Opportunity**: Systematic study of doped DLC for
ultra-high-temperature applications.
```

---

## 6. Citation Management | 引文管理

### 6.1 Organization | 组织

| Phase | Action |
|-------|--------|
| Collection | Export to Zotero/Mendeley |
| Tagging | Add topic tags |
| Notes | Add key findings |
| Organization | Group by topic |

### 6.2 Citation Format | 引用格式

**Numbered | 编号制**:
```markdown
[1] Author, A. et al. (2023). Title. Journal, Volume, Pages.
[2] Author, B. (2022). Title. Journal, Volume, Pages.
```

**Author-Year | 作者-年份制**:
```markdown
Author (2023) found that...
(Author, 2023) demonstrated...
```

---

## 7. Quality Assessment | 质量评估

### 7.1 Paper Evaluation | 论文评估

| Criterion | Weight | Assessment |
|-----------|--------|------------|
| Journal quality | 20% | Q1/Q2 preferred |
| Citation count | 15% | >10 = influential |
| Methodology | 25% | Detailed, reproducible |
| Data | 25% | Quantitative, complete |
| Recency | 15% | 2019-2024 preferred |

### 7.2 Evidence Quality | 证据质量

| Level | Description | Use |
|-------|------------|-----|
| High | Multiple sources, quantitative | Core claims |
| Medium | Single source, detailed | Supporting claims |
| Low | Anecdotal, qualitative | Background only |

---

## 8. Common Sources | 常见来源

### 8.1 Journals | 期刊

| Journal | IF | Coverage |
|---------|-----|----------|
| Tribology International | ~6.5 | Friction, wear |
| Wear | ~5.0 | Wear mechanisms |
| Surface & Coatings Tech | ~5.3 | Coating methods |
| Coatings | ~3.5 | All coatings |

### 8.2 Databases | 数据库

| Database | Content | Access |
|----------|---------|--------|
| Google Scholar | All | Free |
| Web of Science | Quality | Subscription |
| Scopus | Broad | Subscription |
| ArXiv | Preprints | Free |
| PubMed | Biomedical | Free |

---

## 9. Search Example | 搜索示例

### Research Topic | 研究主题

"Development of high-temperature self-lubricating DLC coatings"

### Search Strategy | 搜索策略

```bash
# Step 1: Broad review
"high-temperature DLC coatings review"
→ Collect 5 key review papers

# Step 2: Specific topics
"DLC oxidation high temperature"
"DLC self-lubricating composite"
"DLC MoS2 high temperature"
→ Collect 15-20 papers each

# Step 3: Methods
"RF sputtering DLC optimization"
" PECVD DLC parameters"
→ Collect 10-15 papers

# Step 4: Recent advances (2023-2024)
"site:arxiv.org DLC 2023"
"site:arxiv.org DLC 2024"
→ Collect 5-10 papers

# Step 5: Citation chase
Cited by key papers
→ Collect 10-15 more
```

---

## papers 10. Documentation | 文档

### 10.1 Reading Notes | 阅读笔记

**Template | 模板**:
```markdown
## Paper [ID]
- **Title**: [Full title]
- **Authors**: [Author list]
- **Year**: [Year]
- **Journal**: [Journal, Vol, Pages]
- **DOI**: [Link]

**Key Findings**:
1. [Finding 1]
2. [Finding 2]
3. [Finding 3]

**Methods**:
- [Method 1]
- [Method 2]

**Data**:
- COF: [Value]
- Wear rate: [Value]
- Temperature: [Value]

**Relevance to Proposal**: [How this helps]

**Citations**: [Where to cite in proposal]
```

### 10.2 Summary Document | 总结文档

**Template | 模板**:
```markdown
# Literature Summary: [Topic]

## Current State
[Paragraph summarizing what is known]

## Key Findings
| Finding | Evidence | Quality |
|---------|----------|---------|
| [1] | [Reference] | High |

## Gaps
[Paragraph identifying what is missing]

## Opportunities
[Paragraph on research opportunities]

## Key References
| ID | Citation | Relevance |
|----|----------|-----------|
| 1 | [Full citation] | [Why important] |
```

---

**See also | 参见**:
- [STRUCTURE_GUIDE.md](STRUCTURE_GUIDE.md) - Proposal structure
- [WRITING_STYLE_GUIDE.md](WRITING_STYLE_GUIDE.md) - Writing style
