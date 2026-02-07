# Deposition Methods | 沉积方法详解

This document provides comprehensive coverage of coating deposition methods, their principles, parameters, and applications for literature reviews.

本文档为文献综述提供涂层沉积方法的全面覆盖，包括原理、参数和应用。

---

## 1. Physical Vapor Deposition (PVD) | 物理气相沉积

### 1.1 Magnetron Sputtering | 磁控溅射

#### Principle | 原理

Magnetron sputtering uses argon ions accelerated by electric field to bombard target material, ejecting atoms that deposit on substrate.

| Component | Function |
|-----------|-----------|
| Target | Source material to be deposited |
| Magnetron | Magnetic field to confine plasma |
| Substrate | Sample to be coated |
| Power supply | DC, RF, or pulsed DC |

#### Process Parameters | 工艺参数

| Parameter | Typical Range | Unit | Effect on Coating |
|-----------|---------------|------|-------------------|
| DC Power | 100-2000 | W | Deposition rate |
| RF Power | 50-500 | W | Non-conductive targets |
| Sputtering Pressure | 0.1-10 | Pa | Density, stress |
| Target-substrate distance | 50-150 | mm | Uniformity |
| Substrate Bias | 0-200 | V | Adhesion, density |
| Temperature | RT-500 | °C | Crystallinity |
| Ar Flow | 10-100 | sccm | Plasma stability |
| Deposition Time | 0.5-10 | h | Thickness |

#### Coating Types | 涂层类型

| Target Material | Coating | Application |
|----------------|---------|-------------|
| Graphite | DLC | Tribological |
| MoS₂ | MoS₂ | Solid lubricant |
| Ti | TiN, TiC | Hard coating |
| Cr | CrN | Corrosion resistant |
| Al | Al₂O₃ | Insulation |

#### Advantages | 优势
- Excellent step coverage
- Low substrate damage
- Good adhesion
- Wide material range

#### Limitations | 局限性
- Low deposition rate compared to arc
- Target poisoning possible
- Line-of-sight deposition

---

### 1.2 Cathodic Arc Deposition | 阴极弧沉积

#### Principle | 原理

Cathodic arc uses high-current, low-voltage arc to vaporize material from solid target, producing highly ionized plasma.

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Arc Current | 50-500 | A |
| Arc Voltage | 20-50 | V |
| Pulse Duration | 1-100 | μs |
| Deposition Rate | 1-100 | μm/h |
| Substrate Bias | 20-1000 | V |

#### Advantages | 优势
- Very high deposition rate
- High ionization (80-100%)
- Excellent adhesion
- Dense coatings

#### Limitations | 局限性
- Macroparticle emission
- Target damage
- More complex system

#### Applications | 应用
- Cutting tools (TiN, TiAlN)
- Decorative coatings
- Aerospace components

---

### 1.3 Pulsed Laser Deposition (PLD) | 脉冲激光沉积

#### Principle | 原理

PLD uses high-energy laser pulses to ablate material from target, forming plasma plume that deposits on substrate.

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Laser Energy | 100-1000 | mJ/pulse |
| Repetition Rate | 1-50 | Hz |
| Wavelength | 193-1064 | nm |
| Target-substrate distance | 3-10 | cm |
| Temperature | RT-800 | °C |
| Pressure | 10⁻⁴-100 | Pa |

#### Advantages | 优势
- Excellent stoichiometry transfer
- Clean process
- Precise thickness control
- Multilayer capability

#### Limitations | 局限性
- Low deposition rate
- Small area uniformity
- High equipment cost
- Limited to flat substrates

---

### 1.4 Comparison of PVD Methods | PVD方法对比

| Method | Rate (μm/h) | Ionization | Adhesion | Cost | Complexity |
|--------|--------------|------------|----------|------|------------|
| Sputtering | 0.1-10 | Low-Medium | Good | Medium | Low |
| Arc | 1-100 | High | Excellent | Medium | Medium |
| PLD | 0.01-1 | Medium-High | Very Good | High | High |

---

## 2. Chemical Vapor Deposition (CVD) | 化学气相沉积

### 2.1 Thermal CVD | 热化学气相沉积

#### Principle | 原理

Thermal CVD uses chemical reactions at elevated temperatures to deposit coatings from gas precursors.

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Temperature | 800-1100 | °C |
| Pressure | Atmospheric | atm |
| Gas Flow | 100-1000 | sccm |
| Deposition Rate | 0.1-10 | μm/h |

#### Precursor Gases | 前驱气体

| Coating | Precursors | Reaction |
|---------|------------|----------|
| SiC | SiH₄ + CH₄ | SiH₄ → Si + 2H₂ |
| Si₃N₄ | SiH₄ + NH₃ | 3SiH₄ + 4NH₃ → Si₃N₄ + 12H₂ |
| Diamond | CH₄ + H₂ | CH₄ → C + 2H₂ |

#### Advantages | 优势
- Excellent step coverage
- High purity
- Good conformity
- Large area capability

#### Limitations | 局限性
- High temperature required
- Hazardous gases
- Slow deposition
- Substrate limitation

---

### 2.2 Plasma-Enhanced CVD (PECVD) | 等离子体增强CVD

#### Principle | 原理

PECVD uses plasma to activate chemical reactions at lower temperatures than thermal CVD.

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Temperature | RT-400 | °C |
| RF Power | 10-500 | W |
| Pressure | 0.1-10 | Torr |
| Frequency | 13.56 MHz | - |
| Deposition Rate | 0.1-20 | μm/h |

#### DLC Deposition | DLC沉积

| Gas Mixture | Purpose |
|-------------|---------|
| CH₄ | Carbon source |
| CH₄ + H₂ | Control sp²/sp³ |
| CH₄ + N₂ | N-doped DLC |
| CH₄ + Ar | Plasma stability |

#### Advantages | 优势
- Low temperature deposition
- Good film quality
- Wide material compatibility
- Fast deposition

#### Limitations | 局限性
- Film stress
- Residual gases
- Equipment complexity

---

### 2.3 Atomic Layer Deposition (ALD) | 原子层沉积

#### Principle | 原理

ALD uses sequential, self-limiting surface reactions to deposit coatings atomic layer by atomic layer.

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Temperature | RT-300 | °C |
| Pulse Time | 0.1-10 | s |
| Purge Time | 1-60 | s |
| Deposition Rate | 0.1-1 | Å/cycle |

#### ALD Cycles | ALD循环

```
Cycle 1: Precursor A → Purge → Precursor B → Purge
Cycle 2: Precursor A → Purge → Precursor B → Purge
...
```

#### Advantages | 优势
- Atomic-level control
- Excellent conformity
- Ultra-thin films
- Precise stoichiometry

#### Limitations | 局限性
- Very slow rate
- Limited materials
- Complex precursors

---

### 2.4 Comparison of CVD Methods | CVD方法对比

| Method | Temp (°C) | Rate | Quality | Conformality | Cost |
|--------|------------|------|---------|---------------|------|
| Thermal | 800-1100 | Medium | Excellent | Good | Medium |
| PECVD | RT-400 | High | Very Good | Good | Medium |
| MOCVD | 400-800 | High | Excellent | Fair | High |
| ALD | RT-300 | Very Low | Excellent | Excellent | High |

---

## 3. Thermal Spray Methods | 热喷涂方法

### 3.1 High-Velocity Oxygen Fuel (HVOF) | 高速氧燃料喷涂

#### Principle | 原理

HVOF uses fuel combustion to accelerate powder particles to supersonic velocities for coating deposition.

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Flame Temperature | 2500-3500 | °C |
| Particle Velocity | 300-800 | m/s |
| Spray Distance | 200-400 | mm |
| Deposition Rate | 1-10 | kg/h |
| Coating Thickness | 0.1-1 | mm |

#### Advantages | 优势
- Very high adhesion
- Low porosity (<2%)
- High coating density
- Excellent for wear coatings

#### Limitations | 局限性
- High equipment cost
- Thermal stress
- Large equipment footprint

---

### 3.2 Atmospheric Plasma Spray (APS) | 大气等离子喷涂

#### Principle | 原理

APS uses plasma torch to melt and accelerate powder particles for coating deposition.

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Plasma Temperature | 10000-15000 | K |
| Particle Velocity | 100-300 | m/s |
| Spray Distance | 80-150 | mm |
| Deposition Rate | 0.5-5 | kg/h |
| Coating Thickness | 0.05-0.5 | mm |

#### Advantages | 优势
- Versatile materials
- High deposition rate
- Large area capability
- Moderate cost

#### Limitations | 局限性
- Higher porosity
- Oxide inclusion
- Thermal distortion

---

### 3.3 Cold Spray | 冷喷涂

#### Principle | 原理

Cold spray uses high-pressure gas to accelerate particles above critical velocity for deposition without melting.

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Gas Temperature | 0-800 | °C |
| Gas Pressure | 1-5 | MPa |
| Particle Velocity | 300-1200 | m/s |
| Deposition Rate | 0.1-1 | kg/h |

#### Advantages | 优势
- No oxidation
- Low thermal stress
- High deposition efficiency
- Pure metal coatings

#### Limitations | 局限性
- Limited materials
- Complex process control
- Small area coverage

---

### 3.4 Comparison of Thermal Spray | 热喷涂对比

| Method | Temp | Velocity | Porosity | Adhesion | Cost |
|--------|------|----------|-----------|----------|------|
| HVOF | High | Very High | <2% | Excellent | High |
| APS | Very High | Medium | 5-15% | Good | Medium |
| VPS | High | High | <5% | Excellent | High |
| Cold | Low | Very High | <1% | Very Good | Medium |

---

## 4. Electrochemical Methods | 电化学方法

### 4.1 Electroplating | 电镀

#### Principle | 原理

Electroplating uses electrical current to reduce metal ions from solution onto conductive substrate.

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Current Density | 1-20 | A/dm² |
| Temperature | RT-60 | °C |
| pH | 1-12 | - |
| Deposition Rate | 1-50 | μm/h |
| Thickness | 1-100 | μm |

#### Bath Compositions | 镀液组成

| Coating | Bath Composition |
|---------|-----------------|
| Cr | CrO₃ + H₂SO₄ + additives |
| Ni | NiSO₄ + NiCl₂ + H₃BO₃ |
| Cu | CuSO₄ + H₂SO₄ + Cl⁻ |

#### Advantages | 优势
- Low cost
- High deposition rate
- Good throwing power
- Easy control

#### Limitations | 局限性
- Environmental concerns
- Limited to conductive substrates
- Quality variability

---

### 4.2 Electroless Plating | 化学镀

#### Principle | 原理

Electroless plating uses chemical reduction to deposit metal without electrical current.

| Parameter | Typical Range | Unit |
|-----------|---------------|------|
| Temperature | 80-95 | °C |
| pH | 4-14 | - |
| Deposition Rate | 5-25 | μm/h |
| Thickness | 5-50 | μm |

#### Advantages | 优势
- Non-conductive substrates
- Uniform thickness
- No external power needed
- Good throwing power

#### Limitations | 局限性
- Bath instability
- Costly chemicals
- Waste disposal

---

### 4.3 Comparison | 电化学方法对比

| Method | Conductivity | Uniformity | Cost | Thickness |
|--------|--------------|------------|------|-----------|
| Electroplating | Required | Good | Low | 1-100 μm |
| Electroless | Not required | Excellent | Medium | 5-50 μm |

---

## 5. Summary Comparison | 总结对比

### Deposition Methods Overview | 沉积方法概览

| Category | Method | Rate | Temp | Quality | Cost |
|----------|--------|------|------|---------|------|
| PVD | Sputtering | Low | Low | High | Med |
| PVD | Arc | High | Low | Med | Med |
| CVD | Thermal | Med | High | High | Med |
| CVD | PECVD | High | Low | V.High | Med |
| Spray | HVOF | V.High | High | High | High |
| Spray | APS | High | High | Med | Med |
| Electro | Plating | High | Low | Med | Low |

---

**See also | 参见**:
- [PARAMETER_OPTIMIZATION.md](PARAMETER_OPTIMIZATION.md) - Process optimization
- [CHARACTERIZATION.md](CHARACTERIZATION.md) - Coating characterization
