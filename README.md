# Golden model

The CERG GMU Dilithium RTL implementation from the [GMUCERG repository](https://github.com/GMUCERG/Dilithium) was synthesized using AMD Vivado 2026.1.

## Target device

- Family: Artix-7
- Device: xc7a200tfbg484-3
- Tool: Vivado 2026.1

## Synthesis Results

### Slice Logic

+----------------------------+-------+-------+------------+-----------+-------+
|          Site Type         |  Used | Fixed | Prohibited | Available | Util% |
+----------------------------+-------+-------+------------+-----------+-------+
| Slice LUTs*                | 53683 |     0 |          0 |    134600 | 39.88 |
|   LUT as Logic             | 51844 |     0 |          0 |    134600 | 38.52 |
|   LUT as Memory            |  1839 |     0 |          0 |     46200 |  3.98 |
|     LUT as Distributed RAM |     0 |     0 |            |           |       |
|     LUT as Shift Register  |  1839 |     0 |            |           |       |
| Slice Registers            | 28406 |     0 |          0 |    269200 | 10.55 |
|   Register as Flip Flop    | 28406 |     0 |          0 |    269200 | 10.55 |
|   Register as Latch        |     0 |     0 |          0 |    269200 |  0.00 |
| F7 Muxes                   |  1760 |     0 |          0 |     67300 |  2.62 |
| F8 Muxes                   |   593 |     0 |          0 |     33650 |  1.76 |
| Unique Control Sets        |   268 |       |          0 |     33650 |  0.80 |
+----------------------------+-------+-------+------------+-----------+-------+

### Memory

+-------------------+------+-------+------------+-----------+-------+
|     Site Type     | Used | Fixed | Prohibited | Available | Util% |
+-------------------+------+-------+------------+-----------+-------+
| Block RAM Tile    |   29 |     0 |          0 |       365 |  7.95 |
|   RAMB36/FIFO*    |   29 |     0 |          0 |       365 |  7.95 |
|     RAMB36E1 only |   29 |       |            |           |       |
|   RAMB18          |    0 |     0 |          0 |       730 |  0.00 |
+-------------------+------+-------+------------+-----------+-------+

### DSP

+----------------+------+-------+------------+-----------+-------+
|    Site Type   | Used | Fixed | Prohibited | Available | Util% |
+----------------+------+-------+------------+-----------+-------+
| DSPs           |   16 |     0 |          0 |       740 |  2.16 |
|   DSP48E1 only |   16 |       |            |           |       |
+----------------+------+-------+------------+-----------+-------+

### Primitives

+----------+-------+---------------------+
| Ref Name |  Used | Functional Category |
+----------+-------+---------------------+
| FDRE     | 28395 |        Flop & Latch |
| LUT6     | 26081 |                 LUT |
| LUT5     |  9615 |                 LUT |
| LUT4     |  8503 |                 LUT |
| LUT3     |  8106 |                 LUT |
| LUT2     |  6696 |                 LUT |
| MUXF7    |  1760 |               MuxFx |
| CARRY4   |  1538 |          CarryLogic |
| LUT1     |  1491 |                 LUT |
| SRL16E   |  1124 |  Distributed Memory |
| SRLC32E  |   715 |  Distributed Memory |
| MUXF8    |   593 |               MuxFx |
| IBUF     |    74 |                  IO |
| OBUF     |    66 |                  IO |
| RAMB36E1 |    29 |        Block Memory |
| DSP48E1  |    16 |    Block Arithmetic |
| FDSE     |    11 |        Flop & Latch |
| BUFG     |     1 |               Clock |
+----------+-------+---------------------+

### Power report

| Metric | Power |
|---|---:|
| Total On-Chip Power | 975.355 W |
| Dynamic Power | 973.671 W |
| Device Static Power | 1.684 W |
| Signals | 475.276 W |
| Logic | 468.118 W |
| I/O | 13.133 W |

The power report was generated from the synthesized design using Vivado's default switching activity assumptions.
