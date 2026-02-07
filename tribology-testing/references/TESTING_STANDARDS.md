# Testing Standards | 摩擦学测试标准

This document provides comprehensive coverage of ASTM, ISO, and other standards for tribological testing.

本文档为摩擦学测试提供ASTM、ISO和其他标准的全面覆盖。

---

## 1. ASTM Standards | ASTM标准

### 1.1 Friction Testing | 摩擦测试标准

#### ASTM G99 - Standard Test Method for Wear Testing with a Pin-on-Disk Apparatus

| Aspect | Specification |
|--------|---------------|
| Scope | Pin-on-disk wear testing |
| Load range | 0.1-200 N |
| Speed range | 0.001-5 m/s |
| Track radius | 2-50 mm |
| Temperature | RT to 1000°C (with furnace) |

**Key Requirements | 关键要求**:
- Report: Load, speed, temperature, humidity
- Wear volume calculation: Cross-sectional area × circumference
- COF: Steady-state average
- Replicates: Minimum 3 tests

#### ASTM G133 - Standard Test Method for Linearly Reciprocating Ball-on-Flat Sliding Wear

| Aspect | Specification |
|--------|---------------|
| Scope | Reciprocating ball-on-flat |
| Load range | 0.1-200 N |
| Frequency | 0.01-25 Hz |
| Stroke | 1-50 mm |
| Temperature | RT to 1000°C |

#### ASTM D1894 - Standard Test Method for Static and Kinetic Coefficients of Friction of Plastic Film and Sheeting

| Aspect | Specification |
|--------|---------------|
| Scope | Plastic film testing |
| Speed | 150 ± 30 mm/min |
| Plane angle | 10-80° |
| Load | Weight of sled |

---

### 1.2 Wear Testing | 磨损测试标准

#### ASTM D2596 - Standard Test Method for Measurement of Extreme-Pressure Properties of Lubricating Greases (Four-Ball Method)

| Aspect | Specification |
|--------|---------------|
| Scope | EP properties of greases |
| Ball diameter | 12.7 mm (0.5 inch) |
| Load range | 40-8000 N |
| Speed | 1770 ± 60 rpm (max) |
| Duration | 10 ± 0.2 sec (WSD) |

**Parameters | 参数**:
| Property | Symbol | Unit |
|----------|--------|------|
| Wear Scar Diameter | WSD | mm |
| Load Wear Index | LWI | N |
| Weld Point | WP | N |

#### ASTM D2783 - Standard Test Method for Measurement of Extreme-Pressure Properties of Lubricating Fluids (Four-Ball Method)

| Aspect | Specification |
|--------|---------------|
| Scope | EP fluids |
| Temperature | RT (unless specified) |
| Duration | 10 sec per load |
| Ramp | Load increases by 10% |

#### ASTM G133 - Wear Testing (reciprocating)

| Aspect | Specification |
|--------|---------------|
| Scope | Reciprocating wear |
| Load range | 0.1-200 N |
| Frequency | 0.01-25 Hz |
| Wear volume | Profilometry or interferometry |

---

### 1.3 Adhesion Testing | 附着力测试标准

#### ASTM C1624 - Standard Test Method for Adhesion Strength and Mechanical Failure Modes of Ceramic Coatings by Scratch Testing

| Aspect | Specification |
|--------|---------------|
| Scope | Ceramic coating adhesion |
| Load range | 0.1-200 N |
| Indenter | Rockwell C (200 μm radius) |
| Scratch speed | 1-10 mm/min |
| Scratch length | 1-20 mm |

**Critical Loads | 临界载荷**:
| Load | Description |
|------|-------------|
| Lc1 | First cohesive failure |
| Lc2 | First adhesive failure |
| Lc3 | Complete failure |

#### ASTM D4541 - Standard Test Method for Pull-Off Strength of Coatings Using Portable Adhesion Testers

| Aspect | Specification |
|--------|---------------|
| Scope | Pull-off adhesion |
| Dollies | 20 mm diameter (standard) |
| Pull rate | 1 MPa/s (max) |
| Tensile load | Aligned perpendicular |

---

### 1.4 Mechanical Properties | 机械性能标准

#### ASTM E1921 - Standard Test Method for Determination of Reference Temperature, T₀, for Ferritic Steels in the Transition Range

| Aspect | Specification |
|--------|---------------|
| Scope | Fracture toughness |
| Specimen | SE(B) or C(T) |
| Temperature | Transition range |

---

## 2. ISO Standards | ISO标准

### 2.1 Wear Testing | 磨损测试

#### ISO 20808 - Determination of Hardness and Modulus of Thin Films (Nanoindentation)

| Aspect | Specification |
|--------|---------------|
| Scope | Nanoindentation |
| Load range | 0.1-500 mN |
| Indenter | Berkovich, Vickers |
| Calibration | Fused silica, sapphire |

**Requirements | 要求**:
- Minimum 5 indents per sample
- Spacing: 10× indenter diagonal
- Drift correction: 10-30 s hold
- Report: H, E, H/E, creep

#### ISO 16282 - Determination of Wear Rate of Materials by Pin-on-Disk Testing

| Aspect | Specification |
|--------|---------------|
| Scope | Pin-on-disk wear |
| Load | 1-100 N |
| Speed | 0.01-1 m/s |
| Temperature | RT to 500°C |
| Wear measurement | Profilometry |

---

### 2.2 Surface Characterization | 表面表征

#### ISO 4287 - Terms, Definitions and Surface Texture Parameters

| Parameter | Symbol | Definition |
|-----------|--------|-------------|
| Arithmetic mean roughness | Ra | Integral of |y| |
| Root mean square | Rq | RMS of y |
| Maximum height | Rz | Sum of peak/valley |
| Mean width | RS | Average spacing |

#### ISO 4288 - Rules and Procedures for Measuring Surface Roughness

| Parameter | Cutoff (λc) | Evaluation (λn) |
|-----------|--------------|-------------------|
| Ra 0.02-0.1 μm | 0.25 mm | 1.25 mm |
| Ra 0.1-0.5 μm | 0.8 mm | 4.0 mm |
| Ra 0.5-10 μm | 2.5 mm | 12.5 mm |

#### ISO 25178 - Surface Texture: Areal

| Parameter | Symbol | Definition |
|-----------|--------|-------------|
| Arithmetic mean height | Sa | Areal Ra |
| Root mean square height | Sq | Areal Rq |
| Maximum height | Sz | Areal Rz |

---

## 3. Other Standards | 其他标准

### 3.1 DIN Standards | DIN标准

| Standard | Title | Application |
|----------|-------|-------------|
| DIN 50324 | Tribology Testing | General |
| DIN 4754 | Scratch Testing | Coatings |
| DIN 58399 | Adhesion Testing | Thin films |

### 3.2 JIS Standards | JIS标准

| Standard | Title | Application |
|----------|-------|-------------|
| JIS B 0601 | Surface Roughness | Characterization |
| JIS B 0671 | Wear Testing | Pin-on-disk |
| JIS B 7754 | Scratch Testing | Coatings |

---

## 4. Standards Comparison | 标准对比

| Test | ASTM | ISO | Application |
|------|------|-----|-------------|
| Pin-on-disk wear | G99 | 16282 | General wear |
| Scratch adhesion | C1624 | - | Ceramic coatings |
| Pull-off adhesion | D4541 | - | All coatings |
| Nanoindentation | E2546 | 20808 | Hardness/modulus |
| Roughness | - | 4287/4288 | Surface texture |

---

## 5. Standards Selection Guide | 标准选择指南

### By Test Type | 按测试类型

| Test | Recommended Standard | Key Parameters |
|------|---------------------|----------------|
| Friction COF | ASTM G99, G133 | Load, speed, environment |
| Wear rate | ASTM G99, ISO 16282 | Volume, rate calculation |
| Adhesion | ASTM C1624, D4541 | Critical loads |
| Hardness | ASTM E2546, ISO 20808 | Nanoindentation |
| Roughness | ISO 4287, 4288 | Ra, Rz parameters |

### By Application | 按应用

| Application | Standards | Key Metrics |
|-------------|-----------|-------------|
| Coating evaluation | G99, C1624, D4541 | COF, adhesion, wear |
| Material comparison | G99, D2596 | Relative performance |
| Quality control | G99, 4287 | COF, roughness |
| Research | All relevant | Comprehensive |

---

## 6. Compliance Checklist | 合规检查清单

### Before Testing | 测试前
- [ ] Select appropriate standard
- [ ] Verify equipment compliance
- [ ] Calibrate instruments
- [ ] Document test conditions
- [ ] Prepare samples per standard

### During Testing | 测试中
- [ ] Follow standard procedures
- [ ] Monitor conditions
- [ ] Record all parameters
- [ ] Document anomalies
- [ ] Verify measurements

### After Testing | 测试后
- [ ] Calculate per standard formulas
- [ ] Report required parameters
- [ ] Include uncertainties
- [ ] Reference applicable standards
- [ ] Archive raw data

---

**See also | 参见**:
- [WORKFLOW.md](WORKFLOW.md) - Complete workflow
- [EQUIPMENT.md](EQUIPMENT.md) - Equipment guide
- [DATA_ANALYSIS.md](DATA_ANALYSIS.md) - Analysis methods
