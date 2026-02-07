# Testing Equipment | 测试设备

This document provides comprehensive guidance on tribological testing equipment, their principles, and operating parameters.

本文档为摩擦学测试设备提供全面指导，包括设备原理和操作参数。

---

## 1. Tribometers | 摩擦磨损试验机

### 1.1 Pin-on-Disk Tribometer | 销-盘摩擦磨损试验机

#### Principle | 原理

Pin-on-disk testing involves a stationary pin (or ball) pressed against a rotating disk sample under controlled load, measuring friction force and wear.

| Component | Function |
|-----------|----------|
| Motor | Controls disk rotation |
| Loading system | Applies normal load |
| Force sensor | Measures friction force |
| Sample stage | Holds disk specimen |
| Data acquisition | Records COF vs. time |

#### Specifications | 技术规格

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Load capacity | 0.1-200 | N |
| Rotation speed | 1-5000 | rpm |
| Track radius | 2-50 | mm |
| Friction force range | 0-200 | N |
| Temperature | RT-800 | °C |
| Speed range | 0.01-5 | m/s |

#### Operating Parameters | 操作参数

| Parameter | Typical Value | Notes |
|-----------|---------------|-------|
| Load | 5, 10, 20 | N |
| Speed | 0.1, 0.2 | m/s |
| Duration | 30-120 | min |
| Radius | 15-25 | mm |
| Environment | Air, N₂, vacuum | As required |

#### Leading Manufacturers | 主要厂商

| Manufacturer | Model | Features |
|--------------|-------|----------|
| CSM Instruments | THT | High temperature, vacuum |
| Rtec Instruments | MFT-5000 | Modular, versatile |
| Anton Paar | TRM | Precision, automation |
| Ducom | TRB | Cost-effective |
| NANO-X | NTR² | Nanoscale available |

---

### 1.2 Ball-on-Disk Tribometer | 球-盘摩擦磨损试验机

#### Principle | 原理

Similar to pin-on-disk but uses a ball specimen, commonly used for high-temperature testing and with ceramic counter-bodies.

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Load | 0.1-50 | N |
| Speed | 0.01-0.5 | m/s |
| Temperature | RT-1000 | °C |
| Atmosphere | Air, inert, vacuum | - |

#### Applications | 应用
- High-temperature friction testing
- Ceramic coating evaluation
- Biomedical implant testing
- Lubricant testing

---

### 1.3 4-Ball Tester | 四球摩擦试验机

#### Principle | 原理

Four-ball testing uses three stationary balls clamped together with a fourth rotating ball pressed against them, measuring wear and friction.

| Component | Function |
|-----------|----------|
| 3 stationary balls | Clamped in pot |
| 1 rotating ball | Driven by spindle |
| Loading mechanism | Applies axial load |
| Torque sensor | Measures friction |
| Temperature control | Heats test assembly |

#### Specifications | 技术规格

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Load | 40-8000 | N |
| Speed | 600-3000 | rpm |
| Ball diameter | 12.7 (standard) | mm |
| Test duration | 10 sec - 60 min | - |
| Temperature | RT-300 | °C |

#### Test Types | 测试类型

| Test | Purpose | Duration |
|------|---------|----------|
| Wear Scar Diameter (WSD) | Lubricant evaluation | 60 min |
| Extreme Pressure (EP) | Load-carrying capacity | 10 sec/load |
| Welding Point | Failure load | Ramp test |

---

### 1.4 Reciprocating Tribometer | 往复摩擦试验机

#### Principle | 原理

Linear reciprocating motion simulates back-and-forth sliding, common in engine cylinder and seal testing.

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Load | 1-100 | N |
| Frequency | 1-25 | Hz |
| Stroke length | 1-50 | mm |
| Temperature | RT-600 | °C |

#### Applications | 应用
- Engine cylinder liners
- Seal materials
- Implant testing
- Valve train components

---

## 2. Wear Measurement Equipment | 磨损测量设备

### 2.1 3D Profilometer | 3D轮廓仪

#### Principle | 原理

Optical or stylus-based 3D surface measurement for wear track quantification.

| Technology | Resolution | Advantages |
|------------|------------|------------|
| Optical interferometry | 0.1 nm | Non-contact, fast |
| Confocal microscopy | 1 nm | 3D imaging |
| Stylus profilometry | 1 nm | Direct contact |

#### Specifications | 技术规格

| Parameter | Typical Range |
|-----------|---------------|
| Vertical resolution | 0.1 nm - 1 μm |
| Lateral resolution | 0.1 - 1 μm |
| Measurement range | 1 μm - 10 mm |
| Area | Up to 200×200 mm |

#### Software Features | 软件功能
- Surface roughness analysis (Ra, Rz, Sq)
- Wear volume calculation
- 3D surface visualization
- Batch processing

---

### 2.2 Optical Microscopy | 光学显微镜

| Equipment | Magnification | Application |
|-----------|----------------|-------------|
| Stereo microscope | 5-100× | Low-mag inspection |
| Compound microscope | 50-1000× | High-mag imaging |
| Digital microscope | 20-500× | Image analysis |

#### Wear Scar Measurement | 磨斑测量
```
WSD = (d1 + d2 + d3)/3

Where:
d1, d2, d3 = Three perpendicular diameters
```

---

### 2.3 Scanning Electron Microscopy (SEM) | 扫描电子显微镜

| Mode | Application | Information |
|------|--------------|-------------|
| Secondary electron | Surface morphology | Topography |
| Backscatter | Composition contrast | Phase distribution |
| EDS | Elemental analysis | Composition mapping |
| EBSD | Crystallography | Grain orientation |

#### Sample Preparation | 样品制备
| Method | For | Thickness |
|--------|-----|-----------|
| Carbon coating | Conductive | 10-20 nm |
| Cross-section FIB | Site-specific | <100 nm |
| Ion milling | General | 50-100 nm |

---

### 2.4 Mechanical Testing Machines | 机械测试机

#### Nanoindenter | 纳米压痕仪

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Load | 0.1-500 | mN |
| Displacement | 0-2000 | nm |
| Hardness | 0.1-100 | GPa |
| Modulus | 1-1000 | GPa |

**Indenter Types | 压头类型**:
| Type | Shape | Application |
|------|-------|-------------|
| Berkovich | 3-sided pyramid | General |
| Vickers | Square pyramid | Hard materials |
| Cube-corner | 3-sided | Thin films, small areas |
| Conical | Cone | Plastic deformation |

#### Scratch Tester | 划痕测试仪

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Load range | 0.1-200 | N |
| Scratch speed | 0.1-10 | mm/min |
| Scratch length | 1-50 | mm |
| Acoustic emission | Sensitivity | - |

---

## 3. Environmental Control | 环境控制设备

### 3.1 Temperature Control | 温度控制

| Equipment | Range | Accuracy |
|------------|-------|----------|
| Resistive heating | RT-500°C | ±2°C |
| Induction heating | RT-800°C | ±5°C |
| Furnace | RT-1000°C | ±1°C |
| Liquid nitrogen | -196 to RT | ±1°C |

### 3.2 Atmosphere Control | 气氛控制

| Environment | Control Method | Typical Use |
|--------------|----------------|-------------|
| Air | Open lab | Standard testing |
| Nitrogen | Gas purging | Oxidation studies |
| Argon | Gas purging | Inert atmosphere |
| Vacuum | Pump system | <10^-3 Torr |

### 3.3 Humidity Control | 湿度控制

| Method | Range | Control |
|--------|-------|---------|
| Desiccant | 10-30% RH | Passive |
| Humidifier | 60-90% RH | Active control |
| Environmental chamber | 10-90% RH | Precise |

---

## 4. Supporting Equipment | 辅助设备

### 4.1 Sample Preparation | 样品制备

| Equipment | Function | Specification |
|-----------|----------|---------------|
| Polishing machine | Surface finishing | Down to 0.25 μm |
| Ultrasonic cleaner | Cleaning | 28-40 kHz |
| Balance | Mass measurement | 0.01 mg readability |
| Drying oven | Sample drying | 60-200°C |

### 4.2 Calibration Equipment | 校准设备

| Equipment | For | Frequency |
|-----------|-----|----------|
| Reference weights | Load calibration | Monthly |
| Speed verifier | Speed accuracy | Monthly |
| Temperature probe | Temperature | Quarterly |
| Roughness standard | Profilometer | Weekly |

---

## 5. Data Acquisition | 数据采集

### 5.1 Sensors | 传感器

| Sensor | Signal | Range |
|--------|--------|-------|
| Force transducer | mV/V | 0-200 N |
| Displacement | μm | 0-2000 |
| Temperature | mV, °C | RT-1000°C |
| Acoustic emission | mV | 0-100 |

### 5.2 DAQ Systems | 数据采集系统

| Feature | Typical Spec |
|---------|--------------|
| Sampling rate | 1-100 kHz |
| Resolution | 16-24 bit |
| Channels | 4-32 |
| Software | Real-time display, analysis |

---

## 6. Equipment Selection Guide | 设备选择指南

### By Application | 按应用选择

| Application | Essential Equipment | Optional |
|--------------|---------------------|----------|
| Basic friction/wear | Pin-on-disk, profilometer | SEM |
| High-temperature | HT tribometer, furnace | In-situ Raman |
| Coating adhesion | Nanoindenter, scratch tester | SEM |
| Lubricant testing | 4-ball, pin-on-disk | Tribometer with oil bath |

### By Budget | 按预算选择

| Budget | Recommended |
|--------|--------------|
| Low (<$10K) | Manual tribometer, basic profilometer |
| Medium ($10K-50K) | Automated tribometer, 3D profilometer |
| High (>$50K) | Full characterization suite (SEM, nanoindenter, etc.) |

---

## 7. Maintenance & Calibration | 维护与校准

### 7.1 Routine Maintenance | 日常维护

| Task | Frequency | Notes |
|------|-----------|-------|
| Clean load train | Daily | Remove debris |
| Check calibration | Weekly | Reference standards |
| Lubricate moving parts | Monthly | Per manufacturer |
| Full calibration | Quarterly | Service technician |

### 7.2 Calibration Schedule | 校准周期

| Equipment | Parameter | Interval |
|-----------|-----------|----------|
| Tribometer | Load | Monthly |
| Tribometer | Speed | Monthly |
| Profilometer | Height | Weekly |
| Nanoindenter | Load/displacement | Daily |
| Temperature | Thermocouple | Quarterly |

---

**See also | 参见**:
- [TESTING_STANDARDS.md](TESTING_STANDARDS.md) - Detailed standards
- [WORKFLOW.md](WORKFLOW.md) - Complete workflow
- [DATA_ANALYSIS.md](DATA_ANALYSIS.md) - Analysis methods
