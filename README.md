<h2 align="center">Hi, I'm Ritik</h2>
<p align="center">M.Tech Microelectronics, IIIT Allahabad · Physical Design and Verification</p>

---

I like working on chips from RTL all the way to layout. Most of my recent work is on RISC-V cores: designing them in SystemVerilog, verifying them against reference models, and taking them through synthesis, place and route and sign-off with the Cadence tools. I also build UVM testbenches for clock-domain-crossing designs and full SoCs.

### Projects

**[RV32I 5-Stage Pipelined RISC-V Core: RTL to GDSII](https://github.com/Ritik4388/RV32I-PIPELINED-RTL-TO-GDSII)**
- 5-stage pipeline with forwarding, hazard detection and a 64-entry branch predictor (CPI 1.64 → 1.11)
- Verified against Spike with directed and riscv-dv random tests, on RTL and gate-level netlists
- SKY130 at 50 MHz on a 1.02 × 1.01 mm die, setup +0.33 ns, hold +0.16 ns, clean DRC, LVS and LEC
- Power integrity: 28 mW total, static IR drop under 0.5% of VDD, no EM violations

**[Asynchronous FIFO with UVM Verification]([your-repo-link])**
- Dual-clock FIFO in SystemVerilog with Gray-code pointers, 2-flop synchronizers and registered full/empty flags
- UVM testbench with separate write and read agents (one per clock domain) and a queue-based scoreboard
- Corner cases: write when full, read when empty, simultaneous read/write, pointer wrap-around and reset during traffic
- Tested at several write/read clock ratios (fast-write/slow-read and the reverse)
- SVA for overflow/underflow protection and single-bit Gray pointer transitions; 100% functional coverage

**[RISCFORGE: RISC-V SoC - RTL to Tapeout](https://github.com/Ritik4388/RISCFORGE_1TOPS)** (VSI 1TOPS)
- 5-stage RV32IM core with an AXI-Lite bus, APB bridge and UART, GPIO, SPI, I2C and timer peripherals
- UVM testbenches for the ALU, decoder and hazard unit with constrained-random stimulus, a reference model from the RISC-V spec and 100% code coverage
- Working on SoC-level tests for the UART, GPIO and peripheral registers, where small programs run on the core and UVM agents act as the devices outside the chip
- Found and fixed pipeline hazard and illegal-instruction bugs in the core

### Skills

**Design:** RTL design, pipelined CPU microarchitecture, clock domain crossing (CDC), synchronizers, async FIFOs
**Verification:** UVM, SVA, functional and code coverage, constrained-random stimulus, scoreboards and reference models, SoC-level testing, register testing, Spike, riscv-dv, gate-level simulation
**Protocols and peripherals:** AXI-Lite, APB, UART, SPI, I2C, GPIO
**Physical design:** synthesis, floorplanning, power planning, placement, CTS, routing, STA, IR drop and EM, DRC/LVS, LEC
**Tools:** Cadence Genus, Innovus, Tempus, Voltus, Conformal LEC, PVS, Virtuoso, Xcelium, IMC
**Languages:** Verilog, SystemVerilog, RISC-V assembly, Tcl, Python, Make

### Contact

<a href="https://www.linkedin.com/in/ritik-bharti">LinkedIn</a> · <a href="mailto:ritikbharti43884@gmail.com">Email</a>

