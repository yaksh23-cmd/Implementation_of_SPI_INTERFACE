# Simple SPI Interface: Master & Slave (CPHA/CPOL Support)

## Overview
This project implements a basic SPI interface with master and slave logic using behavioral code. It includes:
- Support for CPHA and CPOL modes
- Basic 3-pin SPI communication (MOSI, MISO, CLK)
- Testbench verification

## SPI Modes Supported
| CPOL | CPHA | Description |
|------|------|-------------|
|  0   |  0   | Mode 0      |
|  0   |  1   | Mode 1      |
|  1   |  0   | Mode 2      |
|  1   |  1   | Mode 3      |

## File Structure
- `master.v` – SPI Master implementation
- `slave.v` – SPI Slave implementation
- `tb_spi.v` – Testbench for simulation
- `README.md` – This file

## Simulation Results
Successfully simulated:
- Single-byte transfer
- CPHA 0/1 handling
- Synchronous behavior under different clock polarity

## Future Work
- Implement chip-select logic (4-pin)
- Add multi-byte FIFO
- Connect to real ADC/DAC (e.g., PMOD DA4)
