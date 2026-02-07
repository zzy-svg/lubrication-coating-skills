# Coating Synthesis Review Workflow | 涂层制备综述工作流

This document details the systematic workflow for writing comprehensive literature reviews on coating deposition and synthesis methods.

本文档详细说明撰写涂层沉积与制备方法综合文献综述的系统性工作流。

---

## Phase 1: Project Initialization | 阶段1：项目初始化

### 创建项目结构 | Create Project Structure

```
project_root/
├── CLAUDE.md              # 写作指南和术语规范
├── IMPLEMENTATION_PLAN.md # 分阶段执行计划
├── manuscript_draft.md   # 主稿件
└── figures/              # 图表占位符
```

### 操作步骤 | Actions

1. **Define review scope**
   - 目标涂层类型 | Target coating types
   - 关注制备方法 | Deposition methods of interest
   - 应用领域 | Application areas

2. **Create CLAUDE.md**
   - 沉积方法术语 | Deposition terminology
   - 工艺参数定义 | Process parameter definitions
   - 性能指标 | Quality metrics

3. **Set objectives**
   - 预期页数 | Target length
   - 目标期刊 | Target journal
   - 时间节点 | Timeline

---

## Phase 2: Literature Collection | 阶段2：文献收集

### 2.1 ArXiv Search | ArXiv搜索

**Categories | 分类**:
- cond-mat.mtrl-sci (Materials Science)
- physics.app-ph (Applied Physics)
- chem-ph (Chemical Physics)

**Example Queries | 示例查询**:
```bash
# PVD methods
"magnetron sputtering DLC coating"
"arc deposition thin film"
"PVD coating optimization"

# CVD methods  
"plasma enhanced CVD DLC"
"thermal CVD coating deposition"
"atomic layer deposition review"

# Thermal spray
"HVOF coating deposition"
"plasma spray coating parameters"
"cold spray aluminum coating"
```

### 2.2 Scholar Search | Scholar搜索

**Keywords | 关键词**:
```markdown
# 沉积方法 | Deposition Methods
"physical vapor deposition" review
"chemical vapor deposition" coating
"thermal spray" process parameters

# 工艺优化 | Process Optimization
"sputtering power effect"
"CVD temperature optimization"
"thermal spray parameter"

# 性能关系 | Property Relationships
"deposition parameters coating hardness"
"sputtering pressure effect"
"CVD gas flow coating quality"
```

### 2.3 Journal-Specific Search | 期刊搜索

| Journal | Focus |
|---------|-------|
| Surface & Coatings Technology | Industrial applications |
| Thin Solid Films | Fundamental research |
| Journal of Materials Science | Materials behavior |
| Vacuum | PVD/CVD methods |
| Surface Engineering | Applied coatings |

### 2.4 Literature Matrix | 文献矩阵

| Method | Subtype | Key Papers | Parameters | Quality | Reference |
|--------|---------|------------|------------|---------|-----------|
| PVD | Sputtering | [refs] | Power, pressure, bias | High | [journal] |
| PVD | Arc | [refs] | Current, voltage | Medium | [journal] |
| CVD | PECVD | [refs] | Power, gas flow | High | [journal] |
| CVD | Thermal | [refs] | Temperature, pressure | High | [journal] |
| Thermal | HVOF | [refs] | Fuel, oxygen | High | [journal] |
| Thermal | Cold spray | [refs] | Pressure, temperature | Medium | [journal] |

---

## Phase 3: Outline Development | 阶段3：大纲制定

### Standard Structure | 标准结构

```markdown
# [Title]: Comprehensive Review of [Deposition Method] for [Coating Type]

## Key Points

## Abstract

## 1. Introduction
### 1.1 Coating importance
### 1.2 Deposition method significance
### 1.3 Review scope

## 2. [Method 1] | 第一种方法
### 2.1 Principle and setup
### 2.2 Process parameters
### 2.3 Coating properties
### 2.4 Advantages and limitations

## 3. [Method 2] | 第二种方法
[Same structure as Method 1]

## 4. [Method 3] | 第三种方法
[Same structure as Method 1]

## 5. Comparative Analysis | 对比分析
### 5.1 Method comparison
### 5.2 Property comparison
### 5.3 Cost analysis

## 6. Process Optimization | 工艺优化
### 6.1 Parameter effects
### 6.2 Design of experiments

## 7. Applications | 应用

## 8. Future Directions | 未来方向

## 9. Conclusion | 结论

## References
```

---

## Phase 4: Section Writing | 阶段4：章节撰写

### Deposition Method Description Template | 沉积方法描述模板

```markdown
### X.X [Method Name]

**Principle | 原理**:
[Brief explanation of the deposition principle - 2-3 sentences]

**Equipment Setup | 设备配置**:
[Schematic description of the deposition system]

**Process Parameters | 工艺参数**:

| Parameter | Typical Range | Unit | Effect on Coating |
|-----------|---------------|------|-------------------|
| Power | 100-2000 | W | Thickness, adhesion |
| Pressure | 0.1-10 | Pa | Density, stress |
| Temperature | RT-500 | °C | Crystallinity, stress |
| Time | 0.1-10 | h | Thickness |
| Bias | 0-200 | V | Density, stress |

**Deposition Steps | 沉积步骤**:
1. [Step 1]
2. [Step 2]
3. [Step 3]

**Coating Properties | 涂层性能**:
| Property | Value | Unit | Condition |
|----------|-------|------|-----------|
| Hardness | 10-30 | GPa | As deposited |
| Thickness | 1-10 | μm | Standard |
| Adhesion | 30-70 | N | Lc2 value |

**Advantages | 优势**:
- [Advantage 1]
- [Advantage 2]

**Limitations | 局限性**:
- [Limitation 1]
- [Limitation 2]

**Applications | 应用**:
- [Application 1]
- [Application 2]

**Key References | 关键参考文献**:
- [Author] ([year]) - Foundational work
- [Author] ([year]) - Recent advance
```

---

## Phase 5: Tables and Figures | 阶段5：表格与图表

### Required Tables | 必需表格

| # | Title | Content |
|---|-------|---------|
| T1 | Deposition Methods Overview | Method, principle, rate, quality |
| T2 | Process Parameters | Parameter, range, effect |
| T3 | Coating Properties | Method, hardness, thickness, adhesion |
| T4 | Cost Comparison | Method, equipment cost, running cost |
| T5 | Application Matching | Application, recommended methods |

### Required Figures | 必需图表

| # | Title | Type |
|---|-------|------|
| F1 | Process schematic | Diagram |
| F2 | Parameter effects | Graph |
| F3 | Property comparison | Bar chart |
| F4 | Coating microstructure | SEM/TEM image |
| F5 | Application examples | Photos |

---

## Phase 6: Quality Assurance | 阶段6：质量保证

### Checklist | 检查清单

| Check Item | Priority | Status |
|------------|----------|--------|
| All methods thoroughly described | High | [ ] |
| Process parameters documented | High | [ ] |
| Property correlations explained | High | [ ] |
| Advantages/limitations balanced | High | [ ] |
| Quantitative data included | High | [ ] |
| Cost analysis included | Medium | [ ] |
| Application guidance provided | High | [ ] |

---

## Phase 7: Incremental Updates | 阶段7：增量更新

### Update Protocol | 更新协议

1. 新方法出现时
   - 分类到适当章节
   - 添加对比表格
   - 更新参考文献

2. 参数优化新发现
   - 更新参数表格
   - 修订影响描述

3. 新应用案例
   - 添加到应用章节
   - 更新应用匹配表

---

## Quick Reference | 快速参考

| Phase | Main Task | Key Outputs |
|-------|-----------|-------------|
| 1 | Initialize | CLAUDE.md, IMPLEMENTATION_PLAN.md |
| 2 | Collect | Literature matrix |
| 3 | Outline | Detailed structure |
| 4 | Write | Section drafts |
| 5 | Visualize | Tables, figures |
| 6 | Verify | Checklist completion |
| 7 | Update | Version log |

---

**See also | 参见**:
- [DEPOSITION_METHODS.md](DEPOSITION_METHODS.md) - Method details
- [PARAMETER_OPTIMIZATION.md](PARAMETER_OPTIMIZATION.md) - Optimization
- [CHARACTERIZATION.md](CHARACTERIZATION.md) - Characterization
