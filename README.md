# Golden Model

The CERG GMU Dilithium RTL implementation from the [GMUCERG repository](https://github.com/GMUCERG/Dilithium) was synthesized using AMD Vivado 2026.1.

## Target Device

- **Family:** Artix-7
- **Device:** xc7a200tfbg484-3
- **Tool:** Vivado 2026.1

## Synthesis Results

### Slice Logic

| Site Type | Used | Fixed | Prohibited | Available | Util% |
| :--- | ---: | ---: | ---: | ---: | ---: |
| Slice LUTs* | 53,683 | 0 | 0 | 134,600 | 39.88% |
| &nbsp;&nbsp;&nbsp;&nbsp;LUT as Logic | 51,844 | 0 | 0 | 134,600 | 38.52% |
| &nbsp;&nbsp;&nbsp;&nbsp;LUT as Memory | 1,839 | 0 | 0 | 46,200 | 3.98% |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;LUT as Distributed RAM | 0 | 0 | - | - | - |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;LUT as Shift Register | 1,839 | 0 | - | - | - |
| Slice Registers | 28,406 | 0 | 0 | 269,200 | 10.55% |
| &nbsp;&nbsp;&nbsp;&nbsp;Register as Flip Flop | 28,406 | 0 | 0 | 269,200 | 10.55% |
| &nbsp;&nbsp;&nbsp;&nbsp;Register as Latch | 0 | 0 | 0 | 269,200 | 0.00% |
| F7 Muxes | 1,760 | 0 | 0 | 67,300 | 2.62% |
| F8 Muxes | 593 | 0 | 0 | 33,650 | 1.76% |
| Unique Control Sets | 268 | - | 0 | 33,650 | 0.80% |

### Memory

| Site Type | Used | Fixed | Prohibited | Available | Util% |
| :--- | ---: | ---: | ---: | ---: | ---: |
| Block RAM Tile | 29 | 0 | 0 | 365 | 7.95% |
| &nbsp;&nbsp;&nbsp;&nbsp;RAMB36/FIFO* | 29 | 0 | 0 | 365 | 7.95% |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;RAMB36E1 only | 29 | - | - | - | - |
| &nbsp;&nbsp;&nbsp;&nbsp;RAMB18 | 0 | 0 | 0 | 730 | 0.00% |

### DSP

| Site Type | Used | Fixed | Prohibited | Available | Util% |
| :--- | ---: | ---: | ---: | ---: | ---: |
| DSPs | 16 | 0 | 0 | 740 | 2.16% |
| &nbsp;&nbsp;&nbsp;&nbsp;DSP48E1 only | 16 | - | - | - | - |

### Primitives

| Ref Name | Used | Functional Category |
| :--- | ---: | :--- |
| FDRE | 28,395 | Flop & Latch |
| LUT6 | 26,081 | LUT |
| LUT5 | 9,615 | LUT |
| LUT4 | 8,503 | LUT |
| LUT3 | 8,106 | LUT |
| LUT2 | 6,696 | LUT |
| MUXF7 | 1,760 | MuxFx |
| CARRY4 | 1,538 | CarryLogic |
| LUT1 | 1,491 | LUT |
| SRL16E | 1,124 | Distributed Memory |
| SRLC32E | 715 | Distributed Memory |
| MUXF8 | 593 | MuxFx |
| IBUF | 74 | IO |
| OBUF | 66 | IO |
| RAMB36E1 | 29 | Block Memory |
| DSP48E1 | 16 | Block Arithmetic |
| FDSE | 11 | Flop & Latch |
| BUFG | 1 | Clock |

### Power Report

| Metric | Power |
| :--- | ---: |
| Total On-Chip Power | 975.355 W |
| Dynamic Power | 973.671 W |
| Device Static Power | 1.684 W |
| Signals | 475.276 W |
| Logic | 468.118 W |
| I/O | 13.133 W |

The power report was generated from the synthesized design using Vivado's default switching activity assumptions.
