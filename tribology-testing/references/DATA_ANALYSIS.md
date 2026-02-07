# Data Analysis | 数据分析

This document provides comprehensive guidance on tribological data analysis methods, statistical treatment, and visualization.

本文档为摩擦学数据分析方法、统计处理和可视化提供全面指导。

---

## 1. Friction Coefficient Analysis | 摩擦系数分析

### 1.1 COF Calculation | COF计算

#### Formula | 公式
```
COF = Friction Force / Normal Load
μ = Ff / Fn

Where:
μ = Coefficient of friction (dimensionless)
Ff = Friction force (N)
Fn = Normal load (N)
```

#### Steady-State COF | 稳态COF

| Method | Description | When to Use |
|--------|-------------|--------------|
| Average | Mean of stable region | Normal conditions |
| Time-weighted | Time-averaged | Varying conditions |
| Median | Median of stable region | Outliers present |

**Calculation Steps | 计算步骤**:
1. Plot COF vs. time
2. Identify steady-state region
3. Calculate mean and standard deviation
4. Report: μ = XX.XX ± XX

### 1.2 COF Variability | COF变异性

| Metric | Formula | Interpretation |
|--------|---------|----------------|
| Mean | Σμi / n | Central tendency |
| Std Dev | √[Σ(μi-μ̄)²/(n-1)] | Spread |
| CV | (SD/Mean) × 100% | Relative variation |
| Peak | Maximum value | Worst case |

### 1.3 Running-in Analysis | 磨合期分析

| Parameter | Definition | Calculation |
|-----------|------------|-------------|
| Running-in time | Time to steady-state | From plot |
| Running-in distance | Distance to steady-state | Speed × Time |
| Initial COF | First stable reading | μ_initial |
| Final COF | Steady-state mean | μ_steady |

---

## 2. Wear Analysis | 磨损分析

### 2.1 Wear Volume Calculation | 磨损体积计算

#### Cross-Sectional Method | 横截面法

```
A = Cross-sectional area
L = Wear track length (circumference)

A = (2/3) × w × d

Where:
w = Track width (mm)
d = Maximum depth (mm)

V = A × L

Where:
V = Wear volume (mm³)
L = 2 × π × r (track radius)
```

#### Interferometry Method | 干涉法

```
V = Σ Δzi × Ai

Where:
Δzi = Depth at point i
Ai = Area element at point i
```

#### Weight Loss Method | 失重法

```
V = (m1 - m2) / ρ

Where:
V = Wear volume (mm³)
m1 = Initial mass (mg)
m2 = Final mass (mg)
ρ = Coating density (mg/mm³)

Note: Account for counter-body transfer
```

### 2.2 Wear Rate Calculation | 磨损率计算

#### Standard Formula | 标准公式
```
WR = V / (Fn × D)

Where:
WR = Wear rate (mm³/N·m)
V = Wear volume (mm³)
Fn = Normal load (N)
D = Sliding distance (m)
```

#### Specific Wear Rate | 比磨损率
```
kw = V / (Fn × D) [mm³/N·m] (standard)

or

kw = Δm / (ρ × Fn × D) [m³/N·m] (SI units)
```

### 2.3 Wear Rate Comparison | 磨损率对比

| Material | Typical Wear Rate | Quality |
|----------|-------------------|---------|
| Excellent | < 10⁻⁸ mm³/N·m | DLC, ceramic |
| Good | 10⁻⁷ - 10⁻⁶ mm³/N·m | Hard coatings |
| Medium | 10⁻⁶ - 10⁻⁵ mm³/N·m | Moderate wear |
| Poor | > 10⁻⁵ mm³/N·m | High wear |

---

## 3. Statistical Analysis | 统计分析

### 3.1 Descriptive Statistics | 描述性统计

| Statistic | Symbol | Formula | Use |
|-----------|--------|---------|-----|
| Mean | x̄ | Σxi / n | Central tendency |
| Median | x̃ | Middle value | Robust central tendency |
| Std Dev | s | √[Σ(xi-x̄)²/(n-1)] | Spread |
| Variance | s² | s² | Squared spread |
| Range | R | max - min | Total spread |

### 3.2 Comparative Statistics | 比较统计

#### t-Test | t检验

| Type | Purpose | Application |
|------|---------|-------------|
| One-sample | Compare to known value | Standard vs. sample |
| Two-sample | Compare two groups | Coating A vs. B |
| Paired | Before/after | Pre/post treatment |

**Formula | 公式**:
```
t = (x̄1 - x̄2) / sp × √(1/n1 + 1/n2)

Where:
sp = Pooled standard deviation
n1, n2 = Sample sizes
```

#### ANOVA | 方差分析

| Source | SS | df | MS | F |
|--------|----|----|----|---|
| Between | SSB | k-1 | MSB = SSB/(k-1) | MSB/MSW |
| Within | SSW | N-k | MSW = SSW/(N-k) | |
| Total | SST | N-1 | | |

**Interpretation | 解读**:
- F > F_critical: Significant difference
- p < 0.05: Statistically significant

### 3.3 Correlation Analysis | 相关性分析

#### Pearson Correlation | 皮尔逊相关
```
r = Σ(xi-x̄)(yi-ȳ) / √[Σ(xi-x̄)² × Σ(yi-ȳ)²]

Where:
r = Correlation coefficient (-1 to 1)
| r | < 0.3: Weak
| r | = 0.3-0.7: Moderate
| r | > 0.7: Strong
```

---

## 4. Wear Mechanism Analysis | 磨损机制分析

### 4.1 Morphology Analysis | 形貌分析

| Mechanism | SEM Observation | EDS Signature |
|-----------|----------------|---------------|
| Adhesive | Material transfer, scoring | Transfer from counter-body |
| Abrasive | Parallel grooves, scratches | Same composition |
| Fatigue | Pits, spalling, cracks | No transfer |
| Oxidational | Oxide debris, glazed layer | Oxygen enrichment |
| Tribochemical | Reaction layer, glaze | Chemical elements |

### 4.2 Quantitative Analysis | 定量分析

| Metric | Method | Interpretation |
|--------|--------|----------------|
| Wear track width | Microscopy | Wear severity |
| Wear scar diameter | Microscopy (4-ball) | Wear extent |
| Debris composition | EDS | Dominant mechanism |
| Surface roughness | Profilometry | Surface damage |

---

## 5. Data Visualization | 数据可视化

### 5.1 Friction Curves | 摩擦曲线

| Plot Type | Information |
|-----------|--------------|
| COF vs. Time | Running-in, steady-state |
| COF vs. Load | Load dependence |
| COF vs. Speed | Speed dependence |
| COF vs. Temperature | Temperature effects |

### 5.2 Wear Plots | 磨损图

| Plot Type | Information |
|-----------|--------------|
| Wear volume vs. Load | Linear regression |
| Wear rate vs. Temperature | Arrhenius plot |
| 3D surface map | Wear track morphology |
| Cross-section profile | Depth profile |

### 5.3 Statistical Plots | 统计图

| Plot Type | Use |
|-----------|-----|
| Box plot | Distribution comparison |
| Error bar plot | Mean ± SD |
| Scatter plot | Correlation |
| Heat map | Multi-parameter |

---

## 6. Report Generation | 报告生成

### 6.1 Results Section | 结果部分

```markdown
## 3. Results | 结果

### 3.1 Friction Performance | 摩擦性能

The friction coefficient was measured under [test conditions].
Steady-state COF values ranged from [min] to [max] with an
average of [mean] ± [SD].

| Sample | Mean COF | SD | Peak COF | n |
|--------|----------|-----|----------|---|
| DLC-A | 0.08 | 0.02 | 0.12 | 5 |
| DLC-B | 0.11 | 0.03 | 0.18 | 5 |
| Steel | 0.65 | 0.05 | 0.75 | 3 |

### 3.2 Wear Performance | 磨损性能

Wear volumes were determined by 3D profilometry. DLC coatings
showed wear rates in the range of [X-Y] × 10⁻⁷ mm³/N·m,
representing a [X]× improvement over uncoated steel.

| Sample | Wear Volume (mm³) | Wear Rate (mm³/N·m) | n |
|--------|--------------------|----------------------|---|
| DLC-A | 0.15 ± 0.05 | (3.0 ± 1.0) × 10⁻⁷ | 5 |
| DLC-B | 0.22 ± 0.08 | (4.4 ± 1.6) × 10⁻⁷ | 5 |
| Steel | 15.5 ± 2.5 | (3.1 ± 0.5) × 10⁻⁴ | 3 |
```

### 6.2 Statistical Analysis Summary | 统计分析总结

| Analysis | Test Statistic | p-value | Significance |
|----------|----------------|---------|--------------|
| COF: DLC-A vs DLC-B | t = 2.34 | 0.04 | p < 0.05* |
| Wear: DLC vs Steel | t = 45.2 | <0.001 | p < 0.001*** |

---

## 7. Uncertainty Analysis | 不确定性分析

### 7.1 Type A Uncertainty | A类不确定度

```
uA = s / √n

Where:
s = Standard deviation
n = Number of measurements
```

### 7.2 Type B Uncertainty | B类不确定度

| Source | Distribution | Division Factor | Calculation |
|--------|--------------|-----------------|-------------|
| Load calibration | Rectangular | √3 | u = a/√3 |
| Length measurement | Rectangular | √3 | u = a/√3 |
| Temperature | Normal | 2 | u = k/2 (k=coverage) |

### 7.3 Combined Uncertainty | 合成不确定度

```
uc = √(uA² + uB1² + uB2² + ...)

Where:
uc = Combined uncertainty
uA = Type A
uBi = Type B components
```

### 7.4 Expanded Uncertainty | 扩展不确定度

```
U = k × uc

Where:
k = Coverage factor (k=2 for 95% confidence)
```

---

## 8. Software Tools | 软件工具

### 8.1 Data Analysis | 数据分析

| Tool | Application | Strengths |
|------|--------------|----------|
| Excel | Basic statistics | Accessibility |
| Origin | Plotting, fitting | Publication quality |
| Python | Advanced analysis | Flexibility |
| SPSS | Statistical tests | ANOVA, regression |
| MATLAB | Signal processing | FFT, filtering |

### 8.2 Wear Analysis | 磨损分析

| Tool | Application |
|------|--------------|
| Gwyddion | Profilometry analysis |
| ImageJ | Microscopy quantification |
| MountainsMap | 3D surface analysis |
| Tribo Analysis | Specialized tribology |

---

## 9. Quality Control | 质量控制

### 9.1 Data Quality Checks | 数据质量检查

| Check | Method | Action if Failed |
|-------|--------|------------------|
| Outliers | Grubbs' test | Remove if confirmed |
| Normal distribution | Shapiro-Wilk | Use non-parametric if not |
| Homogeneity | Levene's test | Use Welch's ANOVA |
| Drift | Trend analysis | Recalibrate |

### 9.2 Reproducibility | 可重复性

| Metric | Acceptance Criteria |
|--------|---------------------|
| COF CV | < 15% |
| Wear rate CV | < 25% |
| Replicates | Minimum 3 |

---

## 10. Template | 模板

### Data Recording Template | 数据记录模板

```markdown
## Test Record | 测试记录

| Field | Value |
|-------|-------|
| Date | YYYY-MM-DD |
| Operator | Name |
| Sample ID | XXX |
| Test Type | Pin-on-disk |

### Test Parameters | 测试参数
| Parameter | Value | Unit |
|-----------|-------|------|
| Load | X | N |
| Speed | X | m/s |
| Temperature | X | °C |
| Duration | X | min |

### Raw Data | 原始数据
| Time (min) | COF | Ff (N) | Fn (N) |
|------------|-----|---------|---------|
| 0 | 0.05 | 0.25 | 5.0 |
| 1 | 0.07 | 0.35 | 5.0 |
| ... | ... | ... | ... |

### Analysis | 分析
| Metric | Value |
|--------|-------|
| Steady-state COF | X.XX ± XX |
| Wear volume | X.XX mm³ |
| Wear rate | X×10^-X mm³/N·m |
| n | X |
```

---

**See also | 参见**:
- [WORKFLOW.md](WORKFLOW.md) - Complete workflow
- [TESTING_STANDARDS.md](TESTING_STANDARDS.md) - Detailed standards
- [EQUIPMENT.md](EQUIPMENT.md) - Equipment guide
