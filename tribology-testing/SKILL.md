---
name: tribology-testing
description: >
  Generate tribological testing reports and data analysis for lubrication coating materials.
  Use when designing experiments, analyzing test data, or reporting tribological testing results.
  Triggers on requests for "wear testing", "friction test", "摩擦学测试",
  "tribology testing", "pin-on-disk", or mentions of tribological testing, friction measurement, wear rate calculation.
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
---

# Tribology Testing Skill

## 摩擦学测试技能

---

## Quick Start | 快速开始

1. **Define test parameters** (load, speed, temperature, environment)
2. **Select test method** (pin-on-disk, ball-on-disk, 4-ball, etc.)
3. **Generate test protocol** with standards
4. **Analyze data** and calculate metrics
5. **Create testing report** with visualizations

**See | 参见**: [references/WORKFLOW.md](references/WORKFLOW.md)

---

## Core Principles | 核心原则

### Test Design | 测试设计

- **Standards-based**: Follow ASTM/ISO standards
- **Systematic**: Controlled variables, clear parameters
- **Reproducible**: Document all conditions
- **Quantitative**: Specific metrics, statistical analysis

### Data Analysis | 数据分析

- **COF calculation**: Average, standard deviation
- **Wear volume**: Profile measurements
- **Wear rate**: Normalized by load and distance
- **Statistics**: Triplicates, error analysis

---

## Test Methods | 测试方法

### 1. Pin-on-Disk | 销-盘法

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Load | 1-20 | N |
| Speed | 0.01-0.5 | m/s |
| Radius | 10-30 | mm |
| Duration | 30-120 | min |

**Standard | 标准**: ASTM G99

### 2. Ball-on-Disk | 球-盘法

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Load | 1-10 | N |
| Speed | 0.01-0.2 | m/s |
| Radius | 10-20 | mm |
| Temperature | RT-500 | °C |

**Standard | 标准**: ASTM G133

### 3. 4-Ball Tester | 四球测试机

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Load | 10-1000 | N |
| Speed | 500-2000 | rpm |
| Temperature | RT-300 | °C |
| Duration | 1-60 | min |

**Standard | 标准**: ASTM D2596, D2783

### 4. Reciprocating | 往复摩擦

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Load | 1-50 | N |
| Frequency | 1-20 | Hz |
| Stroke | 1-20 | mm |
| Duration | 30-120 | min |

**Standard | 标准**: ASTM G133

---

## Test Parameters | 测试参数

### Essential Parameters | 必需参数

| Parameter | Symbol | Unit | Typical Value |
|-----------|--------|------|---------------|
| Normal Load | L | N | 5, 10, 20 |
| Sliding Speed | v | m/s | 0.1, 0.2 |
| Sliding Distance | d | m | 100, 500 |
| Temperature | T | °C | RT, 200, 400 |
| Humidity | RH | % | 50 ± 5 |
| Counter-body | - | - | 100Cr6, Si₃N₄ |

### Optional Parameters | 可选参数

| Parameter | Symbol | Unit | Typical Value |
|-----------|--------|------|---------------|
| Temperature | T | °C | 100-800 |
| Atmosphere | - | - | Air, N₂, Vacuum |
| Lubrication | - | - | Oil, Grease, Dry |

---

## Standard Test Conditions | 标准测试条件

### Ambient Conditions | 环境条件

| Parameter | Value | Tolerance |
|-----------|-------|-----------|
| Temperature | 23°C | ±2°C |
| Humidity | 50% | ±5% RH |
| Atmosphere | Air | Laboratory |

### Reporting Format | 报告格式

```markdown
## Test Conditions
- Load: X N
- Speed: X m/s
- Temperature: X °C
- Humidity: X % RH
- Counter-body: X (material, hardness)

## Results
- Steady-state COF: X.XX ± X.XX
- Wear Rate: X×10^-X mm³/Nm
- Wear Volume: X×10^-X mm³
```

---

## Reference Files | 参考文件

| File | Purpose |
|------|---------|
| [references/WORKFLOW.md](references/WORKFLOW.md) | Complete testing workflow |
| [references/TESTING_STANDARDS.md](references/TESTING_STANDARDS.md) | ASTM/ISO standards |
| [references/EQUIPMENT.md](references/EQUIPMENT.md) | Equipment guide |
| [references/DATA_ANALYSIS.md](references/DATA_ANALYSIS.md) | Data analysis methods |

---

## Usage Examples | 使用示例

### Example 1 | 示例1

**User | 用户**:
```
/tribology-testing
我需要设计一个DLC涂层的耐磨性能测试，
包括不同载荷下的摩擦系数和磨损率测试。
```

**System Response | 系统响应**:
1. Generate test matrix with loads (5N, 10N, 20N)
2. Create test protocol following ASTM G99
3. Define wear measurement procedure
4. Provide data analysis template

### Example 2 | 示例2

**User | 用户**:
```
wear testing report template
Pin-on-disk test for MoS2 coating at high temperature
```

---

**For standards | 标准详情**: [references/TESTING_STANDARDS.md](references/TESTING_STANDARDS.md)
**For equipment | 设备详情**: [references/EQUIPMENT.md](references/EQUIPMENT.md)
