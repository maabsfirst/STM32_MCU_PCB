# STM32F103 Four-Layer PCB Experiment

## Overview

This repository documents my fun experiment designing and assembling my first four-layer PCB based on the STM32F103 microcontroller. After four years of working exclusively with two-layer boards, I decided to push my skills and explore the challenges and benefits of multi-layer board design.

## Design Journey

- **Background**: For most of my projects, two-layer PCBs were sufficient and cost-effective.
- **Challenge**: Transitioning from two layers to four layers introduces layout complexity, signal integrity considerations, power plane management, and more.
- **Solution**: I chose the STM32F103 microcontroller as the core, laid out power and ground planes internally, and routed signals across four layers to optimize space and performance.

## Key Highlights

- **Controller**: STM32F103 (ARM Cortex-M3)
- **Layer Stackup**:
  - Layer 1: Signal
  - Layer 2: Ground Plane
  - Layer 3: Power Plane
  - Layer 4: Signal
- **Features**:
  - Improved signal integrity with dedicated ground and power planes
  - Compact routing for high-density connections
  - Learning-focused design—no specialized impedance control

## Lessons Learned

1. **Multi-layer Routing**: Balancing signal routes across layers is crucial to avoid congestion and interference.
2. **Plane Management**: Properly defining ground and power planes reduces noise and simplifies decoupling strategies.
3. **DFM Considerations**: Four-layer boards require more stringent design rules to meet manufacturer specifications.

## Future Improvements

- Integrate controlled impedance traces for high-speed signals
- Add more decoupling capacitors near critical power pins
- Optimize component placement for easier hand-soldering and rework

## Getting Started

1. Clone this repository:
   ```bash
   git clone https://github.com/your-username/stm32f103-4layer-pcb.git
   ```
2. Open the PCB design files in your preferred EDA tool (e.g., KiCad, Eagle).
3. Review the layer stackup and design guidelines in the `docs/` folder.

## License

Distributed under the MIT License. See [LICENSE](LICENSE) for more details.

---

*I had only worked with two-layer boards over the past four years, because they were sufficient for most of my projects. But as a fun experiment, I designed an STM32F103-based PCB: my first four-layer board and it was quite an adventure. While there’s still plenty of room for improvement, I’m very pleased with how it turned out. It was a fantastic learning experience, and I look forward to tackling more mult
