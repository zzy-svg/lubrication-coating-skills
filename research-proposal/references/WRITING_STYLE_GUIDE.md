# Writing Style Guide | 写作风格指南

This guide provides detailed academic writing guidelines for tribology and coating research proposals, following Nature Reviews style conventions.

本文档为摩擦学和涂层研究计划提供详细的学术写作指导，遵循Nature Reviews风格规范。

---

## 1. Nature Reviews Style | Nature Reviews风格

### 1.1 Core Principles | 核心原则

| Principle | Description | Example |
|-----------|-------------|---------|
| Prose-first | Minimize lists | Use paragraphs |
| Hedging | Tentative claims | "may suggest" |
| Evidence | Support claims | Cite data |
| Clarity | Clear, direct | Active voice |

### 1.2 Sentence Structure | 句子结构

**Recommended | 推荐**:
- Active voice: "We developed..."
- Direct statements: "The coating achieved..."
- Specific claims: "COF of 0.08" not "low friction"
- Varied length: Mix short and long sentences

**Avoid | 避免**:
- Passive overuse: "It was found that..."
- Vague language: "very good", "quite high"
- Nominalization: "make a decision" → "decide"

**Example Revisions | 修改示例**:

| Weak | Strong |
|------|--------|
| It was found that DLC coatings showed low friction | DLC coatings achieved COF of 0.05-0.15 |
| The experiments showed good results | The coatings demonstrated 85% wear reduction |
| It is believed that temperature affects performance | Increasing temperature from 25°C to 400°C increased COF by 40% |

---

## 2. Hedging Language | 谨慎表达语言

### 2.1 Appropriate Hedging | 适当谨慎表达

| Purpose | Language | Example |
|---------|----------|---------|
| Claims with evidence | "demonstrates", "shows" | "The results demonstrate..." |
| Probable findings | "suggests", "indicates" | "The data suggests..." |
| Tentative claims | "may", "might", "could" | "Temperature may affect..." |
| Limitations | "appears to", "seems to" | "The coating appears to..." |

### 2.2 Strong Claims | 强表达

Use when evidence is strong:
- "demonstrates"
- "proves" (rarely)
- "confirms"
- "establishes"

### 2.3 Weak Claims | 弱表达

Use when evidence is preliminary:
- "suggests"
- "indicates"
- "may"
- "might"

**Example | 示例**:

```markdown
# Strong evidence (multiple studies)
The tribological benefits of DLC coatings have been extensively
demonstrated [1-5].

# Moderate evidence (some studies)
MoS₂ addition may improve high-temperature stability [6].

# Preliminary evidence (single study)
These preliminary results suggest potential for further optimization [7].
```

---

## 3. Quantitative Reporting | 定量报告

### 3.1 Numbers | 数字

| Type | Format | Example |
|------|--------|---------|
| Numbers < 10 | Words | "three coatings" |
| Numbers ≥ 10 | Numerals | "15 samples" |
| Measurements | Numerals + units | "5.2 mm" |
| Ranges | Numerals | "10-20 samples" |

### 3.2 Statistics | 统计

| Item | Format | Example |
|------|--------|---------|
| Mean ± SD | "mean ± SD" | "0.15 ± 0.03" |
| Range | "range" | "0.08-0.25" |
| Percentages | Numerals | "15%" not "fifteen percent" |
| P-values | Italic p | "p < 0.05" |

### 3.3 Units | 单位

| Quantity | SI Unit | Abbreviation |
|----------|---------|---------------|
| Length | meter | m, cm, mm, μm, nm |
| Mass | kilogram | kg, g, mg, μg |
| Pressure | pascal | Pa, kPa, MPa |
| Temperature | kelvin | K, °C |
| Time | second | s, min, h |
| Force | newton | N |
| Hardness | pascal | GPa |
| Coefficient | - | dimensionless |

---

## 4. Citation Style | 引用风格

### 4.1 In-Text Citations | 文中引用

| Situation | Format | Example |
|-----------|--------|---------|
| Single reference | [#] | "...as shown [1]" |
| Multiple | [#-#] | "...reported [2-5]" |
| Discontinuous | [#, #] | "...studies [6, 8]" |
| Author-year | Author et al. (Year) | "...Li et al. (2023)" |

### 4.2 Reference List | 参考文献列表

**Journal Article | 期刊论文**:
```markdown
[1] Author, A. & Author, B. Title of the article. Journal Name Volume, Pages (Year).
```

**Example | 示例**:
```markdown
[1] Zhang, Y. et al. High-temperature tribological properties of DLC coatings.
Tribology International 178, 108542 (2023).

[2] Liu, J. & Wang, H. Machine learning for coating optimization. Surf. Coat.
Technol. 457, 129-142 (2022).
```

---

## 5. Section-Specific Writing | 逐节写作指导

### 5.1 Introduction | 引言

**Opening Hook | 开场**:
```markdown
# Good opening
Friction accounts for approximately 23% of global energy consumption
in mechanical systems, representing a significant opportunity for
energy savings through improved tribological materials [1, 2].

# Weak opening
This proposal is about coatings. Coatings are important for many
applications. This research will help.
```

**Problem Statement | 问题陈述**:
```markdown
# Effective problem statement
Despite significant advances in DLC coating technology, achieving
stable low friction (COF < 0.10) at temperatures above 400°C
remains challenging due to oxidation and structural degradation
[3-5]. Current approaches, including doping and multilayer designs,
have shown partial success but lack comprehensive optimization.

# Weak problem statement
Current DLC coatings have some problems. They don't work well
at high temperatures. We need to fix this.
```

### 5.2 Objectives | 目标

**Format | 格式**:
```markdown
# Specific objective
Develop TiAlN/MoS₂ composite coatings with COF < 0.15 and wear rate
< 10⁻⁶ mm³/Nm at 500°C through systematic optimization of MoS₂
content (5-30 wt%) and deposition parameters.

# Vague objective
Improve coating properties for high-temperature use.
```

### 5.3 Methods | 方法

**Tense and Voice | 时态和语态**:
| Section | Tense | Voice |
|---------|-------|-------|
| Methods | Past | Passive acceptable |
| Results | Past | Active preferred |
| Discussion | Present | Active |

**Example | 示例**:
```markdown
# Methods section
Coatings were deposited using RF magnetron sputtering (Kurt J.
Lesker, Proline). A 3-inch MoS₂ target (99.9% purity) was used
at 150 W power, with substrate temperature maintained at 400°C.

# Results section
The coatings achieved COF values ranging from 0.08 to 0.25
depending on MoS₂ content. The minimum COF of 0.08 ± 0.02 was
observed at 15 wt% MoS₂ content.
```

### 5.4 Expected Outcomes | 预期成果

**Balance claims | 平衡声明**:
```markdown
# Appropriate hedging
We anticipate that the optimized coatings will demonstrate
improved high-temperature stability, with potential applications
in aerospace and automotive components.

# Overclaiming
We will definitely create the best coating ever made that will
revolutionize the industry.
```

---

## 6. Common Errors and Fixes | 常见错误与修正

### 6.1 Language Issues | 语言问题

| Error | Fix |
|-------|-----|
| "It is found that" | "The results show" |
| "In order to" | "To" |
| "At the present time" | "Currently" |
| "Due to the fact that" | "Because" |
| "Has been shown to be" | "Is" |

### 6.2 Structure Issues | 结构问题

| Error | Fix |
|-------|-----|
| Long paragraphs | Split into 2-3 paragraphs |
| Bullet overuse | Convert to prose |
| Citation clusters | Spread references |
| Undefined terms | Define first use |

### 6.3 Citation Issues | 引用问题

| Error | Fix |
|-------|-----|
| Too many citations | Select most relevant (3-5) |
| Old references | Prioritize recent (2019-2024) |
| Single-source claims | Add supporting evidence |
| Broken format | Check journal format |

---

## 7. Word Choice | 词汇选择

### 7.1 Preferred Terms | 推荐术语

| Avoid | Use |
|-------|-----|
| "very" | Specific quantity |
| "good/bad" | Quantitative descriptor |
| "things" | Specific nouns |
| "shown" | "demonstrated", "revealed" |
| "big" | "large", specific dimension |

### 7.2 Technical Vocabulary | 技术词汇

| Term | Use When |
|------|----------|
| "coefficient of friction" (COF) | General friction |
| "wear rate" | Volume loss per distance |
| "adhesion strength" | Coating-substrate bond |
| "tribological properties" | Friction and wear |
| "deposition" | Coating process |
| "characterization" | Analysis techniques |

---

## 8. Tone and Voice | 语气和语态

### 8.1 Professional Tone | 专业语气

| Approach | Example |
|----------|---------|
| Confident but humble | "The results suggest..." |
| Objective | Present data without emotion |
| Precise | Specific numbers, conditions |
| Balanced | Acknowledge limitations |

### 8.2 Active vs Passive | 主动vs被动

**Use Active When | 主动语态使用场景**:
- Clear performer of action
- Emphasizing the researcher
- Improving readability

**Use Passive When | 被动语态使用场景**:
- Standard method description
- Equipment is the subject
- Emphasizing the action/process

**Example | 示例**:
```markdown
# Active (preferred)
We deposited the coatings using RF magnetron sputtering.

# Passive (acceptable)
The coatings were deposited using RF magnetron sputtering.
```

---

## 9. Length Guidelines | 长度指导

### By Section | 按章节

| Section | Percentage | Words (5000 total) |
|---------|------------|-------------------|
| Abstract | 5% | 250 |
| Introduction | 20% | 1000 |
| Objectives | 5% | 250 |
| Literature Review | 20% | 1000 |
| Methodology | 25% | 1250 |
| Expected Outcomes | 10% | 500 |
| Timeline | 10% | 500 |
| Significance | 5% | 250 |

---

## 10. Checklist | 检查清单

### Before Submission | 投稿前
- [ ] Consistent terminology throughout
- [ ] Proper hedging language used
- [ ] Quantitative data presented clearly
- [ ] Citations formatted correctly
- [ ] No spelling/grammar errors
- [ ] Passive/active voice consistent
- [ ] Appropriate section lengths

---

**See also | 参见**:
- [STRUCTURE_GUIDE.md](STRUCTURE_GUIDE.md) - Section structure
- [LITERATURE_WORKFLOW.md](LITERATURE_WORKFLOW.md) - Literature
- [assets/proposal_scaffold_en.md](../assets/proposal_scaffold_en.md) - Template
