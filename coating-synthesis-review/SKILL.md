---
name: coating-synthesis-review
description: >
  Write comprehensive literature reviews on coating deposition and synthesis methods for lubrication coatings.
  Use when writing reviews on PVD, CVD, thermal spray, electroplating methods, or coating preparation processes.
  Triggers on requests for "coating preparation", "deposition methods", "PVD CVD review", "制备方法综述",
  "涂层沉积综述", or mentions of coating synthesis, deposition techniques, or manufacturing processes.
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
---

# Coating Synthesis Review Skill

## 涂层制备方法综述撰写技能

---

## Quick Start | 快速开始

1. **Initialize project** with three core files:
   - `CLAUDE.md` - Writing guidelines and terminology
   - `IMPLEMENTATION_PLAN.md` - Staged execution plan
   - `manuscript_draft.md` - Main manuscript

2. **Follow the 7-phase workflow** (see [references/WORKFLOW.md](references/WORKFLOW.md))

3. **Use deposition method templates** (see [references/DEPOSITION_METHODS.md](references/DEPOSITION_METHODS.md))

---

## Core Principles | 核心原则

### Writing Style | 写作风格

- **Process descriptions**: Detailed step-by-step explanations
- **Parameter emphasis**: Critical process parameters and their effects
- **Comparative analysis**: Compare methods, advantages, limitations
- **Application matching**: Match methods to target applications

### Required Elements | 必需元素

- **Process flow diagrams** with key parameters
- **Comparison tables** for each deposition category
- **Property correlations**: Process parameters → coating properties
- **Quality metrics**: Deposition rate, thickness, adhesion
- **References**: 60-100 typical, organized by method

### Deposition Method Template | 沉积方法模板

```markdown
### X.X [Method Name]

**Principle | 原理**: [Brief description of the deposition principle]

**Process Parameters | 工艺参数**:
| Parameter | Typical Range | Effect on Coating |
|-----------|---------------|-------------------|
| [Param 1] | [Range] | [Effect] |
| [Param 2] | [Range] | [Effect] |

**Advantages | 优势**:
- [Advantage 1]
- [Advantage 2]

**Limitations | 局限性**:
- [Limitation 1]
- [Limitation 2]

**Applications | 应用**:
- [Application 1]
- [Application 2]
```

---

## Deposition Methods | 沉积方法

### 1. Physical Vapor Deposition (PVD) | 物理气相沉积

| Method | Principle | Deposition Rate | Quality | Cost |
|--------|-----------|-----------------|---------|------|
| Sputtering | Ion bombardment | Low-Medium | High | Medium |
| Arc Deposition | Arc evaporation | High | Medium | Medium |
| PLD | Laser ablation | Low | Very High | High |
| E-Beam | Electron beam | High | High | High |

### 2. Chemical Vapor Deposition (CVD) | 化学气相沉积

| Method | Temperature | Coating Quality | Substrate | Cost |
|--------|-------------|-----------------|-----------|------|
| Thermal CVD | High (800-1100°C) | High | Heat-resistant | Medium |
| PECVD | Low (RT-400°C) | Medium-High | All | Medium |
| MOCVD | Medium (400-800°C) | Very High | Semiconductors | High |
| ALD | Low (RT-300°C) | Excellent | All | High |

### 3. Thermal Spray | 热喷涂

| Method | Temperature | Deposition Rate | Adhesion | Cost |
|--------|-------------|-----------------|----------|------|
| HVOF | Very High | Very High | Excellent | High |
| APS | High | High | Good | Medium |
| VPS | Very High | High | Excellent | High |
| Cold Spray | Low | Medium | Good | Medium |

### 4. Electrochemical Methods | 电化学方法

| Method | Temperature | Thickness | Conductivity | Cost |
|--------|-------------|-----------|-------------|------|
| Electroplating | Room Temp | 1-100 μm | Required | Low |
| Electroless | 80-95°C | 5-50 μm | Not required | Medium |
| Anodization | Room Temp | 1-50 μm | Metal only | Low |

---

## Standard Review Structure | 标准综述结构

```markdown
# [Title]: Deposition Methods and Synthesis Strategies for [Coating Type] Coatings

## Key Points | 关键发现

## Abstract | 摘要

## 1. Introduction | 引言
### 1.1 Importance of Deposition Methods
### 1.2 Review Scope and Objectives

## 2. Physical Vapor Deposition | 物理气相沉积
### 2.1 Sputtering
### 2.2 Arc Deposition
### 2.3 Pulsed Laser Deposition
### 2.4 Comparison of PVD Methods

## 3. Chemical Vapor Deposition | 化学气相沉积
### 3.1 Thermal CVD
### 3.2 Plasma-Enhanced CVD
### 3.3 Atomic Layer Deposition
### 3.4 Comparison of CVD Methods

## 4. Thermal Spray Methods | 热喷涂方法
### 4.1 HVOF
### 4.2 Atmospheric Plasma Spray
### 4.3 Cold Spray

## 5. Electrochemical Deposition | 电化学沉积
### 5.1 Electroplating
### 5.2 Electroless Plating

## 6. Process Parameter Optimization | 工艺参数优化
### 6.1 Parameter Effects on Properties
### 6.2 Design of Experiments

## 7. Characterization Methods | 表征方法
### 7.1 Structural Analysis
### 7.2 Mechanical Properties
### 7.3 Tribological Testing

## 8. Comparative Analysis | 对比分析

## 9. Future Directions | 未来方向

## 10. Conclusion | 结论

## References | 参考文献
```

---

## Key Metrics | 关键指标

| Metric | Description | Typical Range |
|--------|-------------|----------------|
| Deposition Rate | Coating thickness per unit time | 0.1-100 μm/h |
| Adhesion Strength | Coating-substrate bond | 10-100 N (Lc2) |
| Hardness | Coating hardness | 1-80 GPa |
| Thickness | Coating thickness | 0.1-100 μm |
| Deposition Temperature | Process temperature | RT-1100°C |
| Step Coverage | Conformal coverage | 50-100% |
| Growth Rate | Crystal growth speed | nm/min - μm/h |

---

## Reference Files | 参考文件

| File | Purpose |
|------|---------|
| [references/WORKFLOW.md](references/WORKFLOW.md) | Detailed 7-phase workflow |
| [references/DEPOSITION_METHODS.md](references/DEPOSITION_METHODS.md) | Method comparison |
| [references/PARAMETER_OPTIMIZATION.md](references/PARAMETER_OPTIMIZATION.md) | Process parameters |
| [references/CHARACTERIZATION.md](references/CHARACTERIZATION.md) | Characterization |
| [references/QUALITY_CHECKLIST.md](references/QUALITY_CHECKLIST.md) | Quality checklist |

---

## Usage Examples | 使用示例

### Example 1 | 示例1

**User | 用户**:
```
/coating-synthesis-review
我想写一篇关于"PVD涂层制备工艺"的综述文章，
重点关注磁控溅射和阴极弧沉积方法的比较。
```

### Example 2 | 示例2

**User | 用户**:
```
coating synthesis review
Review paper on CVD methods for DLC coating deposition,
including PECVD and thermal CVD comparison
```

---

**For detailed methods | 详细方法参见**: [references/DEPOSITION_METHODS.md](references/DEPOSITION_METHODS.md)
