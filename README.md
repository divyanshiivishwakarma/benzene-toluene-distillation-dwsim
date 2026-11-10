# Simulation and Performance Analysis of a Binary Distillation Column Using DWSIM

## 1. Project Overview

This project focuses on the steady-state simulation and performance analysis of a benzene–toluene distillation column using DWSIM.

The main objective is to investigate how changes in reflux ratio affect product purity and energy consumption while maintaining constant feed conditions and column configuration.

The project demonstrates fundamental chemical engineering concepts, including vapor–liquid equilibrium, mass and energy balances, distillation, and process performance analysis.

## 2. Simulation Details

| Parameter | Value |
|---|---|
| Simulation Software | DWSIM |
| Components | Benzene and Toluene |
| Thermodynamic Model | Raoult's Law |
| Feed Flow Rate | 100 kmol/h |
| Feed Composition | 50 mol% Benzene, 50 mol% Toluene |
| Feed Temperature | 70°C (343.15 K) |
| Feed Pressure | 101325 Pa (approximately 1 atm) |
| Column Top Pressure | 101325 Pa (approximately 1 atm) |
| Column Pressure Drop | 0 Pa (assumed) |
| Number of Stages | 20 |
| Feed Stage | Stage 10 |
| Condenser Type | Total Condenser |
| Reboiler Specification | Bottom Product Molar Flow (13.8889 mol/s) |
| Reflux Ratios Studied | 2, 3 and 4 |

## 3. Methodology

The simulation was developed and analyzed through the following steps:

1. Selected benzene and toluene as the chemical components and Raoult's Law as the thermodynamic model.
2. Created an equimolar benzene–toluene feed stream and specified its temperature, pressure, and flow rate.
3. Configured a 20-stage distillation column with a total condenser and reboiler.
4. Connected the feed, distillate, bottoms, and energy streams.
5. Performed steady-state simulations at reflux ratios of 2, 3, and 4 while keeping the other operating specifications constant.
6. Recorded product compositions and condenser/reboiler energy duties.
7. Compared the simulated operating conditions to evaluate the relationship between separation performance and energy requirements.
8. Verified the overall mass and energy balances for the reflux ratio of 4.

## 4. Simulation Results

The following results were obtained from DWSIM:

| Parameter | R = 2 | R = 3 | R = 4 |
|---|---:|---:|---:|
| Benzene Purity in Distillate (%) | 99.30 | 99.75 | 99.86 |
| Toluene Purity in Bottoms (%) | 99.30 | 99.75 | 99.86 |
| Condenser Duty Magnitude (kW) | 1282.90 | 1708.96 | 2135.74 |
| Reboiler Duty (kW) | 1408.79 | 1835.25 | 2262.12 |

### 4.1 Effect of Reflux Ratio on Product Purity

![Reflux Ratio vs Product Purity](graphs/reflux_vs_purity.png)

Increasing the reflux ratio improved the separation of benzene and toluene.

- At R = 2, both products achieved approximately 99.30 mol% purity.
- At R = 3, product purity increased to approximately 99.75 mol%.
- At R = 4, product purity increased further to approximately 99.86 mol%.

However, the improvement in purity became smaller at higher reflux ratios.

### 4.2 Effect of Reflux Ratio on Energy Requirements

![Reflux Ratio vs Energy Duty](graphs/reflux_vs_energy_duty.png)

Both condenser and reboiler duties increased with increasing reflux ratio.

Increasing the reflux ratio from 3 to 4:

- Increased the reboiler duty by approximately 23.3%.
- Increased the condenser duty magnitude by approximately 25.0%.
- Improved product purity by only approximately 0.10 percentage points.

These findings demonstrate the trade-off between separation performance and energy consumption.

## 5. Mass and Energy Balance Verification

The overall mass and energy balances were checked using DWSIM for the R = 4 operating condition.

### Mass Balance

| Stream | Mass Flow Rate (kg/s) |
|---|---:|
| Feed | 2.36459 |
| Distillate | 1.08516 |
| Bottoms | 1.27943 |
| Total Outlet | 2.36459 |

The total mass entering the system approximately equals the total mass leaving the system, confirming mass conservation within numerical precision.

### Energy Balance

The DWSIM balance summary reported approximately equal total energy inflows and outflows of 3307.24 kW, with a negligible difference.

This supports the consistency of the simulated operating condition with the overall energy balance.

## 6. Key Findings

- The distillation column achieved up to 99.86 mol% purity for both benzene and toluene under the simulated conditions.
- Increasing reflux ratio improved separation performance but also increased heating and cooling requirements.
- Higher reflux ratios produced diminishing improvements in product purity.
- For an assumed product purity requirement of **99.5 mol%**, R = 3 was the lowest-energy operating condition among the three tested cases that satisfied this requirement.
- Overall mass and energy balances were verified for the R = 4 operating condition.

## 7. Conclusion

A steady-state benzene–toluene distillation column was successfully simulated using DWSIM.

The study demonstrated that increasing the reflux ratio improves product purity but also increases energy requirements.

Among the three operating conditions investigated, a reflux ratio of 3 provided a suitable balance between product purity and energy demand for an assumed minimum purity requirement of 99.5 mol%.

The results demonstrate the importance of evaluating separation efficiency alongside utility requirements when selecting distillation operating conditions.

## 8. Future Scope

The project can be extended through:

- Studying the effect of feed-stage location on product purity.
- Investigating different numbers of theoretical stages.
- Performing a more detailed sensitivity analysis over additional reflux ratios.
- Estimating utility costs and conducting economic optimization.
- Evaluating alternative thermodynamic models and column operating conditions.

## 9. Tools and Concepts Used

**Software:** DWSIM

**Chemical Engineering Concepts:**
- Binary Distillation
- Vapor–Liquid Equilibrium
- Thermodynamic Property Models
- Mass and Energy Balances
- Reflux Ratio
- Condenser and Reboiler Duties
- Process Simulation and Performance Analysis
