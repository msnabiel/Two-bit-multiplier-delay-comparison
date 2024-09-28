# Two-Bit Multiplier Delay Comparison: PLA vs. Conventional Logic in Cadence Virtuoso

This repository contains the files and scripts used to perform a comparison analysis of the **delay characteristics** of a two-bit multiplier circuit designed using **Programmable Logic Array (PLA)** and **conventional logic gates** in **Cadence Virtuoso**.

## Project Overview

The project focuses on measuring and comparing the **propagation delay** between the two approaches (PLA and conventional logic). The delay is analyzed based on factors such as gate count, technology node, and interconnects, using **Cadence Virtuoso** for schematic design and simulation.

### Key Concepts:
- **PLA (Programmable Logic Array):** A customizable logic structure that allows flexible design but introduces higher delays due to programmable connections.
- **Conventional Logic Gates:** A hardwired implementation using standard gates such as AND, OR, and XOR, offering faster signal propagation at the cost of design flexibility.

## Repository Structure

```
/two-bit-multiplier-delay-comparison
│
├── /schematics/                   # Contains Cadence Virtuoso schematic files for both PLA and conventional logic circuits
│   ├── pla_multiplier.sch          # Schematic for two-bit multiplier using PLA
│   ├── conventional_multiplier.sch # Schematic for two-bit multiplier using conventional logic
│
├── /simulation_results/            # Contains simulation results and delay analysis data
│   ├── pla_delay_report.csv        # Delay data for PLA multiplier
│   ├── conventional_delay_report.csv # Delay data for conventional logic multiplier
│
├── /scripts/                       # Python/Skill scripts for automating simulation runs
│   └── run_simulations.py          # Python script to run and collect simulation results
│
├── README.md                       # Project documentation
└── LICENSE                         # License information for the project
```

## Tools Used

- **Cadence Virtuoso:** For schematic design and transient delay analysis.
- **Python Scripts:** For automating simulation runs and collecting data.
  
## How to Use

1. Clone the repository:
   ```
   git clone https://github.com/msnabiel/two-bit-multiplier-delay-comparison.git
   ```
   
2. Open **Cadence Virtuoso** and load the schematics from the `/schematics/` folder.

3. Perform a **transient analysis** for both the PLA-based and conventional logic-based two-bit multiplier circuits to observe and compare delays.

4. You can also use the Python script provided in `/scripts/` to automate the simulation process:
   ```
   python run_simulations.py
   ```

5. The results of the simulation will be stored in `/simulation_results/` as CSV files for analysis.

## Results

After running the simulations, you can compare the delay data between the two implementations:
- **PLA Multiplier:** Typically has higher delay due to programmable interconnects.
- **Conventional Logic Multiplier:** Offers lower delay due to hardwired connections.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
