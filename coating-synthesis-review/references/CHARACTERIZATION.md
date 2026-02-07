# Coating Characterization | 涂层表征方法

This document provides comprehensive coverage of characterization techniques for coating analysis.

本文档为涂层分析提供表征方法的全面覆盖。

---

## 1. Structural Analysis | 结构分析

### 1.1 X-Ray Diffraction (XRD) | X射线衍射

| Application | Information Obtained |
|-------------|---------------------|
| Phase identification | Crystal structure |
| Crystallite size | Scherrer equation |
| Residual stress | sin²ψ method |
| Texture analysis | Pole figures |

**Parameters | 参数**:
| Parameter | Typical Value | Unit |
|-----------|---------------|------|
| 2θ range | 20-90 | degrees |
| Scan speed | 1-10 | deg/min |
| Step size | 0.02-0.1 | degrees |
| Cu Kα | 1.5406 | Å |

**Common Phases | 常见物相**:
| Coating | 2θ (°) | (hkl) |
|---------|---------|-------|
| TiN | 36.7 | (111) |
| TiN | 42.6 | (200) |
| DLC (amorphous) | Broad peak 20-30 | - |
| MoS₂ (002) | 14.5 | (002) |

---

### 1.2 Raman Spectroscopy | 拉曼光谱

| Application | Information Obtained |
|-------------|---------------------|
| DLC bonding | D-band, G-band |
| Stress measurement | Peak shift |
| Crystallinity | Peak intensity |
| Phase identification | Characteristic peaks |

**DLC Analysis | DLC分析**:
| Band | Position (cm⁻¹) | Meaning |
|------|-----------------|---------|
| D-band | 1350-1380 | sp² disorder |
| G-band | 1580-1600 | sp² graphitic |
| ID/IG ratio | - | Disorder level |

**DLC Quality Assessment | DLC质量评估**:
```
ID/IG < 0.4: High sp³, high quality
ID/IG 0.4-0.8: Medium quality
ID/IG > 0.8: High sp², low quality
```

---

### 1.3 Transmission Electron Microscopy (TEM) | 透射电镜

| Technique | Information |
|-----------|-------------|
| HRTEM | Atomic structure |
| SAED | Crystal structure |
| STEM-EDS | Elemental mapping |
| EELS | Electronic structure |

**Sample Preparation | 样品制备**:
| Method | Thickness | Application |
|--------|-----------|-------------|
| FIB | <100 nm | Site-specific |
| Ion milling | 50-100 nm | General |
| Electro-polishing | <100 nm | Metals |

---

### 1.4 X-Ray Photoelectron Spectroscopy (XPS) | X射线光电子能谱

| Application | Information Obtained |
|-------------|---------------------|
| Surface chemistry | Elemental composition |
| Chemical state | Bonding environment |
| Depth profiling | Interface analysis |
| Contamination | Surface impurities |

**Common Binding Energies | 常见结合能**:
| Element | Compound | BE (eV) |
|---------|----------|----------|
| C 1s | C-C sp³ | 285.0 |
| C 1s | C=C sp² | 284.5 |
| C 1s | C-O | 286.5 |
| N 1s | TiN | 397.0 |
| O 1s | TiO₂ | 530.0 |

---

## 2. Mechanical Properties | 机械性能

### 2.1 Nanoindentation | 纳米压入

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Load | 0.1-500 | mN |
| Depth | 50-2000 | nm |
| Loading rate | 0.1-1 | mN/s |
| Hold time | 10-60 | s |

**Hardness Calculation | 硬度计算**:
```
H = P / A

Where:
H = Hardness (GPa)
P = Maximum load (mN)
A = Contact area (mm²)
```

**Elastic Modulus | 弹性模量**:
```
E* = (π/2) × (dP/dh) / √A

Where:
E* = Reduced modulus
dP/dh = Load-displacement slope
A = Contact area
```

**Oliver-Pharr Method | Oliver-Pharr方法**:
| Step | Description |
|------|-------------|
| 1 | Load to maximum |
| 2 | Hold for creep |
| 3 | Unload to 10% |
| 4 | Fit unload curve |
| 5 | Calculate stiffness |

---

### 2.2 Scratch Testing | 划痕测试

| Critical Load | Description |
|---------------|-------------|
| Lc1 | First cohesive failure |
| Lc2 | First adhesive failure |
| Lc3 | Complete coating failure |

**Failure Modes | 失效模式**:
| Mode | Description | Indication |
|------|-------------|------------|
| Cohesive | Inside coating | Spallation |
| Adhesive | Interface | Delamination |
| Combined | Mixed | Buckling |

---

### 2.3 Adhesion Testing | 附着力测试

| Method | Information | Standard |
|--------|-------------|----------|
| Pull-off | Tensile strength | ASTM D4541 |
| Scratch | Critical load | ASTM C1624 |
| Indentation | Interfacial toughness | ASTM E1921 |
| Bending | Flexible substrates | ASTM D522 |

---

### 2.4 Tribological Testing | 摩擦学测试

| Test | Information | Standard |
|------|-------------|----------|
| Pin-on-disk | COF, wear rate | ASTM G99 |
| Ball-on-disk | Friction, wear | ASTM G133 |
| Reciprocating | Linear friction | ASTM G133 |
| 4-ball | EP performance | ASTM D2596 |

---

## 3. Morphology Analysis | 形貌分析

### 3.1 Scanning Electron Microscopy (SEM) | 扫描电镜

| Mode | Application |
|------|-------------|
| SE | Surface topography |
| BSE | Composition contrast |
| EDS | Elemental analysis |
| EBSD | Crystallographic |

**Imaging Parameters | 成像参数**:
| Parameter | Typical Value |
|-----------|---------------|
| Voltage | 5-20 kV |
| Working distance | 5-15 mm |
| Magnification | 100-100,000× |
| Current | 0.1-10 nA |

---

### 3.2 Atomic Force Microscopy (AFM) | 原子力显微镜

| Mode | Application |
|------|-------------|
| Contact | Hard surfaces |
| Tapping | Soft materials |
| PeakForce | Mechanical properties |
| Conductive | Electrical properties |

**Surface Parameters | 表面参数**:
| Parameter | Symbol | Unit | Description |
|-----------|--------|------|-------------|
| Roughness | Ra | nm | Arithmetic mean |
| RMS | Rq | nm | Root mean square |
| Peak-to-valley | Rt | nm | Max height difference |

---

### 3.3 3D Profilometry | 3D轮廓仪

| Technique | Vertical Resolution | Lateral Resolution |
|-----------|---------------------|-------------------|
| Optical | 0.1 nm | 0.5 μm |
| Stylus | 1 nm | 0.1 μm |
| Confocal | 1 nm | 0.2 μm |

**Wear Volume Calculation | 磨损体积计算**:
```
V = A × L

Where:
V = Wear volume (mm³)
A = Cross-sectional area (mm²)
L = Wear track length (mm)
```

---

## 4. Composition Analysis | 成分分析

### 4.1 Energy Dispersive Spectroscopy (EDS) | 能谱分析

| Information | Detection Limit | Spatial Resolution |
|-------------|-----------------|--------------------|
| Elements | >0.1 wt% | 1-10 μm |
| Mapping | >0.5 wt% | 1-10 μm |
| Line scan | >0.1 wt% | 0.1-1 μm |

---

### 4.2 Secondary Ion Mass Spectrometry (SIMS) | 二次离子质谱

| Mode | Information | Depth Resolution |
|------|-------------|-----------------|
| Dynamic SIMS | Concentration profile | 1-10 nm |
| Static SIMS | Surface composition | Monolayer |
| ToF-SIMS | Molecular information | 0.5 nm |

---

### 4.3 Glow Discharge Optical Emission Spectroscopy (GDOES) | 辉光放电光谱

| Application | Detection Limit | Depth Resolution |
|--------------|-----------------|------------------|
| Concentration depth profiling | ppm | 1-10 nm |
| Interface analysis | ppm | 1-5 nm |
| Coating thickness | - | 0.1 μm |

---

## 5. Testing Standards Summary | 测试标准汇总

| Property | Technique | Standard |
|----------|-----------|----------|
| Hardness | Nanoindentation | ISO 14577 |
| Modulus | Nanoindentation | ISO 14577 |
| Scratch | Scratch test | ASTM C1624 |
| Adhesion | Pull-off | ASTM D4541 |
| Friction | Pin-on-disk | ASTM G99 |
| Wear | Pin-on-disk | ASTM G99 |
| Roughness | Profilometry | ISO 4287 |
| Thickness | Cross-section | ASTM B487 |

---

## 6. Characterization Flowchart | 表征流程图

```
Coating Sample
     ↓
[Non-destructive | 非破坏性]
     ├─ Optical microscopy
     ├─ SEM
     ├─ XRD
     └─ Raman
     ↓
[Mechanical | 机械性能]
     ├─ Nanoindentation
     ├─ Scratch test
     └─ Tribological test
     ↓
[Structural | 结构]
     ├─ TEM
     ├─ XPS
     └─ SIMS
     ↓
[Report | 报告]
     └─ Complete characterization
```

---

## 7. Typical Characterization Protocol | 典型表征方案

### DLC Coating | DLC涂层

| Step | Technique | Information |
|------|-----------|-------------|
| 1 | SEM | Surface morphology |
| 2 | Raman | sp³/sp² ratio |
| 3 | XPS | Surface chemistry |
| 4 | Nanoindentation | Hardness, modulus |
| 5 | Tribology | COF, wear rate |
| 6 | Cross-section | Thickness |

### Hard Coating | 硬质涂层

| Step | Technique | Information |
|------|-----------|-------------|
| 1 | XRD | Phase identification |
| 2 | SEM | Cross-section |
| 3 | EDS | Composition |
| 4 | Nanoindentation | Hardness |
| 5 | Scratch | Adhesion |
| 6 | Tribology | Wear resistance |

---

**See also | 参见**:
- [METRICS.md](../tribology-review/references/METRICS.md) - Performance metrics
- [DEPOSITION_METHODS.md](DEPOSITION_METHODS.md) - Deposition methods
