# Tribological Metrics and Evaluation Standards | 摩擦学指标与评价标准

This document provides comprehensive coverage of tribological performance metrics, testing methods, and evaluation standards for lubrication coating research.

本文档为润滑涂层研究提供摩擦学性能指标、测试方法和评价标准的全面覆盖。

---

## 1. Friction Performance Metrics | 摩擦性能指标

### 1.1 Coefficient of Friction (COF) | 摩擦系数

#### Definition | 定义

```
COF = Friction Force / Normal Load
μ = F / N
```

#### COF Types | COF类型

| Type | Symbol | Description | Typical Range |
|------|--------|-------------|---------------|
| Static COF | μs | Friction at rest (initiation of motion) | Higher than dynamic |
| Dynamic COF | μd | Friction during sustained motion | More stable value |
| Transient COF | μt | During running-in period | Variable |

#### Typical COF Values | 典型COF值

| Condition | COF Range | Interpretation |
|-----------|------------|----------------|
| Dry sliding (steel) | 0.60 - 0.80 | High friction |
| Lubricated (oil) | 0.05 - 0.15 | Moderate friction |
| Boundary lubrication | 0.10 - 0.30 | Mixed regime |
| DLC coating (dry) | 0.02 - 0.15 | Ultra-low friction |
| MoS₂ coating (vacuum) | 0.01 - 0.03 | Excellent |
| PTFE coating | 0.04 - 0.20 | Low friction |

#### Measurement Conditions | 测量条件

| Parameter | Common Values | Units |
|-----------|---------------|-------|
| Normal Load | 1 - 50 | N |
| Sliding Speed | 0.01 - 1.0 | m/s |
| Sliding Distance | 10 - 1000 | m |
| Temperature | RT - 800 | °C |
| Humidity | 20 - 80 | % RH |

### 1.2 Friction Curves | 摩擦曲线

#### Typical Friction Curve | 典型摩擦曲线

```
COF
  │
  │  ╭─── Running-in period (variable)
  │ ╱
  │╱
  │╲  Steady-state friction (stable)
  │ ╲
  │  ╰─── End of test
  └────────────────────── Sliding Distance/Time
```

#### Analysis Parameters | 分析参数

| Parameter | Description | Unit |
|-----------|-------------|------|
| Running-in time | Time to reach steady-state | s or m |
| Steady-state COF | Average COF after running-in | - |
| COF fluctuation | Standard deviation | - |
| Friction peak | Maximum COF observed | - |
| Stability index | Consistency measure | % |

---

## 2. Wear Performance Metrics | 磨损性能指标

### 2.1 Wear Rate (WR) | 磨损率

#### Definition | 定义

```
WR = Wear Volume / (Normal Load × Sliding Distance)
WR = V / (L × D)

Units: mm³/(N·m) or m³/(N·m)
```

#### Archard Wear Equation | Archard磨损方程

```
V = K × (F × s) / H

Where:
V = Wear volume (mm³)
K = Wear coefficient (dimensionless)
F = Normal load (N)
s = Sliding distance (m)
H = Hardness (Pa or HV)
```

#### Typical Wear Rates | 典型磨损率

| Material/Coating | Wear Rate | Unit | Quality |
|------------------|-----------|------|----------|
| Uncoated steel | 10^-3 - 10^-4 | mm³/Nm | Poor |
| Hard coating (TiN) | 10^-5 - 10^-6 | mm³/Nm | Good |
| DLC coating | 10^-7 - 10^-8 | mm³/Nm | Excellent |
| Self-lubricating | 10^-6 - 10^-7 | mm³/Nm | Very good |
| MoS₂ coating | 10^-6 - 10^-5 | mm³/Nm | Good |

### 2.2 Wear Volume Calculation | 磨损体积计算

#### Profilometry Method | 轮廓仪法

```
W = A × L

Where:
W = Wear volume (mm³)
A = Cross-sectional area (mm²)
L = Wear track length (mm)
```

#### Weight Loss Method | 失重法

```
W = (m₁ - m₂) / ρ

Where:
W = Wear volume (mm³)
m₁ = Initial mass (mg)
m₂ = Final mass (mg)
ρ = Density (mg/mm³)

Note: Consider counter-body transfer
```

### 2.3 Wear Mechanisms | 磨损机制

| Mechanism | Description | Indicators |
|-----------|-------------|------------|
| Adhesive wear | Material transfer between surfaces | Scoring, galling, transfer films |
| Abrasive wear | Ploughing or cutting by hard particles | Scratches, grooves, debris |
| Fatigue wear | Surface/sub-surface cracking | Pitting, spalling, delamination |
| Oxidational wear | Oxide formation and removal | Oxide debris, tribolayers |
| Tribochemical wear | Chemical reaction with environment | Reaction layers, selective dissolution |
| Corrosive wear | Combined chemical and mechanical | Corrosion products |

---

## 3. Mechanical Properties | 机械性能

### 3.1 Hardness | 硬度

| Method | Symbol | Load Range | Application |
|--------|--------|------------|-------------|
| Vickers | HV | 0.01 - 50 kgf | General |
| Knoop | HK | 0.01 - 1 kgf | Thin films |
| Nanoindentation | H | 0.1 - 500 mN | Coatings < 1 μm |

#### Hardness Values | 硬度值

| Material | Hardness (GPa) | Method |
|----------|----------------|--------|
| DLC (ta-C) | 40 - 80 | Nanoindentation |
| DLC (a-C) | 20 - 30 | Nanoindentation |
| TiAlN | 25 - 35 | Vickers |
| TiN | 20 - 25 | Vickers |
| CrN | 15 - 20 | Vickers |
| MoS₂ | 1 - 10 | Nanoindentation |
| Steel (substrate) | 5 - 10 | Vickers |

### 3.2 Elastic Modulus | 弹性模量

| Material | E-Modulus (GPa) | Method |
|----------|-----------------|--------|
| ta-C | 400 - 600 | Nanoindentation |
| a-C | 200 - 300 | Nanoindentation |
| TiN | 400 - 500 | Nanoindentation |
| Steel substrate | 200 - 220 | Standard |

### 3.3 H/E Ratio | 硬弹比

#### Definition | 定义

```
H/E Ratio = Hardness / Elastic Modulus
```

#### Significance | 意义

| H/E Range | Interpretation |
|-----------|----------------|
| < 0.05 | Low elastic recovery |
| 0.05 - 0.10 | Moderate |
| 0.10 - 0.15 | Good elastic recovery |
| > 0.15 | Excellent |

#### Typical Values | 典型值

| Coating | H/E Ratio | Wear Resistance |
|---------|-----------|----------------|
| ta-C | 0.10 - 0.15 | Excellent |
| TiAlN | 0.06 - 0.08 | Very good |
| DLC (a-C:H) | 0.07 - 0.10 | Very good |
| CrN | 0.05 - 0.07 | Good |

### 3.4 Adhesion Strength | 附着力

#### Scratch Test | 划痕测试

| Critical Load | Symbol | Description |
|---------------|--------|-------------|
| Lc1 | Cohesive failure | Cohesive strength of coating |
| Lc2 | Adhesive failure | Adhesion to substrate |
| Lc3 | Scratch through | Complete coating failure |

#### Typical Lc Values | 典型Lc值

| Coating/Substrate | Lc1 (N) | Lc2 (N) | Lc3 (N) |
|-------------------|---------|---------|----------|
| TiN on steel | 10 - 20 | 30 - 60 | 50 - 100 |
| DLC on steel | 15 - 25 | 40 - 70 | 60 - 120 |
| CrN on steel | 12 - 22 | 35 - 65 | 55 - 110 |

---

## 4. Testing Standards | 测试标准

### 4.1 ASTM Standards | ASTM标准

| Standard | Test Method | Application |
|----------|-------------|-------------|
| ASTM G99 | Pin-on-disk wear testing | General wear measurement |
| ASTM G132 | Pin-on-block testing | Friction measurement |
| ASTM D1894 | Coefficient of friction | Plastic films |
| ASTM D3363 | Pencil hardness | Coating hardness |
| ASTM D4541 | Pull-off adhesion | Adhesion strength |
| ASTM D4060 | Taber abrasion | Abrasion resistance |
| ASTM D5178 | Mar resistance | Surface marring |
| ASTM D2794 | Reverse impact | Coating adhesion |
| ASTM D3359 | Cross-cut tape | Adhesion classification |
| ASTM B571 | Adhesion | Metallic coatings |

### 4.2 ISO Standards | ISO标准

| Standard | Test Method | Application |
|----------|-------------|-------------|
| ISO 20808 | Nanoindentation | Hardness and modulus |
| ISO 4287 | Surface roughness | Ra, Rz parameters |
| ISO 4288 | Surface texture | Measurement procedure |
| ISO 16282 | Wear testing | Pin-on-disk |
| ISO 5436-1 | Calibration | Surface standards |
| EN 1071-13 | Adhesion testing | Ceramic coatings |

### 4.3 Other Standards | 其他标准

| Standard | Origin | Application |
|----------|--------|-------------|
| DIN 50324 | Germany | Tribology testing |
| JIS B 0601 | Japan | Surface roughness |
| VDI 3822 | Germany | Coating characterization |

---

## 5. Test Parameters | 测试参数

### 5.1 Typical Test Conditions | 典型测试条件

| Parameter | Range | Typical Value | Units |
|-----------|-------|---------------|-------|
| Normal Load | 1 - 50 | 5, 10, 20 | N |
| Sliding Speed | 0.01 - 1.0 | 0.1, 0.2 | m/s |
| Sliding Distance | 10 - 1000 | 100, 500 | m |
| Temperature | RT - 800 | RT, 200, 400 | °C |
| Humidity | 20 - 80 | 50 | % RH |
| Counter-body | Steel, Si₃N₄, Al₂O₃ | 100Cr6, Si₃N₄ | - |
| Ball diameter | 3 - 10 | 6 | mm |
| Track radius | 10 - 30 | 20 | mm |

### 5.2 Environmental Factors | 环境因素

| Factor | Effect on DLC | Effect on MoS₂ |
|--------|---------------|-----------------|
| Humidity (↑) | Slight COF increase | Significant COF increase |
| Temperature (↑) | Oxidation risk | Oxidation above 350°C |
| Vacuum | Excellent | Excellent |
| Inert gas | Good | Good | Good |

---

## 6. Surface Characterization | 表面表征

### 6.1 Morphology | 形貌

| Technique | Information | Resolution |
|-----------|-------------|------------|
| SEM | Surface morphology, wear tracks | nm - μm |
| AFM | Nanoscale topography | nm |
| Optical Microscopy | General observation | μm |
| 3D Profilometry | Wear volume, surface height | nm - μm |

### 6.2 Composition | 成分

| Technique | Information | Depth |
|-----------|------------|-------|
| XPS | Surface chemistry, bonding | 1 - 10 nm |
| EDS | Elemental composition | 1 - μm |
| AES | Depth profiling | nm - μm |
| SIMS | Trace elements, isotopes | nm |
| Raman | Carbon bonding (sp²/sp³) | μm |

### 6.3 Structure | 结构

| Technique | Information | Application |
|-----------|-------------|-------------|
| XRD | Crystal structure | Phase identification |
| TEM | Microstructure, defects | Nanoscale structure |
| SAED | Crystal structure | Selected area diffraction |
| HRTEM | Lattice imaging | Atomic structure |

---

## 7. Performance Metrics Summary | 性能指标汇总

### Coating Selection Guide | 涂层选择指南

| Application | Priority 1 | Priority 2 | COF Target | Wear Rate Target |
|-------------|------------|------------|------------|------------------|
| Precision parts | DLC | TiN | < 0.1 | < 10^-7 mm³/Nm |
| Cutting tools | TiAlN | AlCrN | 0.3-0.5 | < 10^-7 mm³/Nm |
| Space | MoS₂ | WS₂ | < 0.05 | < 10^-6 mm³/Nm |
| Automotive | DLC (a-C:H) | CrN | 0.05-0.15 | < 10^-6 mm³/Nm |
| Biomedical | DLC | TiN | 0.1-0.2 | < 10^-7 mm³/Nm |

### Quality Metrics | 质量指标

| Metric | Excellent | Good | Acceptable | Poor |
|--------|-----------|------|------------|------|
| COF (dry) | < 0.05 | 0.05 - 0.15 | 0.15 - 0.30 | > 0.30 |
| Wear Rate | < 10^-7 | 10^-7 - 10^-6 | 10^-6 - 10^-5 | > 10^-5 |
| Hardness | > 40 GPa | 20 - 40 GPa | 10 - 20 GPa | < 10 GPa |
| Adhesion (Lc2) | > 70 N | 40 - 70 N | 20 - 40 N | < 20 N |
| H/E Ratio | > 0.12 | 0.08 - 0.12 | 0.05 - 0.08 | < 0.05 |

---

## 8. Data Reporting Format | 数据报告格式

### Standard Test Report | 标准测试报告

```markdown
## Test Conditions | 测试条件
- Load: X N
- Speed: X m/s
- Distance: X m
- Temperature: X °C
- Humidity: X % RH
- Counter-body: X (material, hardness)

## Results | 结果
- Steady-state COF: X.XX ± X.XX
- Wear Rate: X×10^-X mm³/Nm
- Wear Volume: X×10^-X mm³
- Running-in Distance: X m

## Wear Mechanism | 磨损机制
[Description of dominant wear mechanism based on microscopy]

## Remarks | 备注
[Any special observations or deviations from standard conditions]
```

---

**See also | 参见**:
- [DOMAINS.md](DOMAINS.md) - Coating categories
- [WORKFLOW.md](WORKFLOW.md) - Testing workflow
- [TESTING_STANDARDS.md](../tribology-testing/references/TESTING_STANDARDS.md) - Detailed standards
