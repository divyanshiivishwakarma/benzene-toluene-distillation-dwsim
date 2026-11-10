
# Simulation and Performance Analysis of a Binary Distillation Column Using DWSIM

## Project Overview

This project focuses on the steady-state simulation of a benzene–toluene distillation column using DWSIM. The objective is to study the effect of reflux ratio on product purity and energy requirements.

## Simulation Details

- **Software:** DWSIM
- **Components:** Benzene and Toluene
- **Thermodynamic Model:** Raoult's Law
- **Feed Flow Rate:** 100 kmol/h
- **Feed Composition:** 50 mol% Benzene, 50 mol% Toluene
- **Feed Temperature:** 70°C
- **Operating Pressure:** 1 atm
- **Number of Stages:** 20
- **Feed Stage:** 10
- **Condenser:** Total condenser

## Methodology

1. Developed a steady-state binary distillation simulation in DWSIM.
2. Configured the feed, distillation column, condenser and reboiler.
3. Simulated the system at reflux ratios of 2, 3 and 4.
4. Recorded product compositions and heating/cooling duties.
5. Compared separation performance and energy requirements.
6. Verified overall mass and energy balances for the R = 4 case.

## Simulation Results

| Parameter | R = 2 | R = 3 | R = 4 |
|---|---:|---:|---:|
| Benzene Purity (%) | 99.30 | 99.75 | 99.86 |
| Toluene Purity (%) | 99.30 | 99.75 | 99.86 |
| Condenser Duty (kW) | 1282.90 | 1708.96 | 2135.74 |
| Reboiler Duty (kW) | 1408.79 | 1835.25 | 2262.12 |

## Key Findings

- Increasing the reflux ratio improved the separation of benzene and toluene.
- Higher reflux ratios increased both condenser and reboiler duties.
- Increasing reflux from 3 to 4 produced a relatively small purity improvement compared with the additional energy requirement.
- Among the three simulated conditions, R = 3 met an illustrative 99.5 mol% purity target with lower energy demand than R = 4.

## Conclusion

The project demonstrates the trade-off between separation efficiency and energy consumption in a binary distillation column. The simulation results highlight the importance of selecting suitable operating conditions rather than maximizing reflux ratio.

## Future Scope

- Investigating the effect of feed-stage location.
- Studying the influence of the number of theoretical stages.
- Performing further energy and operating-cost optimization.
