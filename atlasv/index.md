---
layout: default
title: "Atlas V"
description: "Sirf Atlas V short description"
nav_order: 1        
has_children: true  
has_toc: true       
parent: Atlas SoCs
---

# Atlas V: A short glance

## Computing Cores
- 500 MHz ARM11 with 16KB D-cache and I-cache, 16KB D-TCM and I-TCM (Official is 500MHz, however is overclockable up to 750)
- 250 MHz Enhanced DSP for GPS
- Low power advanced 65nm process
  
## Memory Subsystem
- 64-bit 250 MHz system bus with 16 DMA channels
- 1.8V 16-bit mDDR-333/DDR2-400 support
  
## Advanced Autonomous GPS
- 64 channels
- -161 dBm sensitivity
- Able to acquire and track Galileo signals on all channels
  
## Display, Graphics, and Multimedia
- Up to 800x480 at 16 bits color
- RGB565 or 16-bit CPU I/F TFT LCD panel
- Hardware VPP (Video Post Processor) for de-interlace, scalar, color space conversion
- Two hardware overlay layers
  
## Peripherals and Interfaces

### Power Integration
- Two switching DC/DC for core (1000mA) and DRAM (500mA)
- One high PSRR and low noise 300mA LDO for I/O and peripheral
- One high PSRR and low noise 150mA LDO for analog power
- One high PSRR and low noise 10mA LDO for PLL
- One high PSRR and low noise 100mA LDO for RF
- One high PSRR and low noise 10mA LDO for RTC

### Audio Integration
- One mono differential audio output with 93db SNR and 80db THD (“A” weighted)
- One stereo audio output with 85db SNR and 70db THD (“A” weighted) connectivity

### Connectivity
- One dedicated AC97/I2S interface
- Two dedicated UART ports
- Two USP ports for PCM, DSP, I2S, SPI, UART mode
- Two I2C ports
- 12-bit ADC with 4-wire touch screen controller and 3 channel analog input, stream measurement mode for low cost audio input

### NAND Flash Storage
- 8-bit NAND flash interface with 12/24bit configurable BCH HW ECC support
- Supports direct boot from SLC or MLC NAND
- Supports SLC 512B, 2KB, 4KB page size
- Supports MLC 2KB, 4KB, 8KB page size

### SD/MMC/MMC+ Controller
- SDIO support for Wi-Fi, DVB-T/DVB-H/T--DMB/S-DMB
- Supports direct boot from SD/MMC+ Managed NAND
- Two 8-bit SD1.01/SD 2.1/MMC4.3 ports
- Two 4-bit SD1.01/SD2.1/MMC4.3 ports

### USB Connectivity
- One USB 2.0 High Speed interfaces with on chip PHY
- Can be Host, Device or OTG
- Transfer up to 480Mbps

### Packaging
- 10mm x 13mm 285 ball TFBGA with .65mm pitch
### Temperature Range
- -20°C ~ +70°C extended commercial grade

---
## System Memory Mapping

| Address Range | Usage | Resource Size |
| ------------- | ----- | ------------- |
| 0xE000_0000~FFFF_FFFF | Zero Bank | 512 MB |
| 0xC000_0000~DFFF_FFFF | System Memory | 512 MB |
| 0x8000_0000~BFFF_FFFF | Internal Registers | 1 GB |
| 0x7000_0000~7000_FFFF | ITCM | 64 KB |
| 0x7001_0000~7001_FFFF | DTCM | 64 KB |
| 0x7002_0000~7FFF_FFFF | - | Reserved |
| 0x6000_0000~6FFF_FFFF | PCI Flash/ROM | 256 MB |
| 0x5000_0000~5FFF_FFFF | Other PCI Devices | 256 MB |
| 0x4800_0000~4FFF_FFFF | DSP Shared Memory | 128 MB |
| 0x4000_0000~47FF_FFFF | - | 128 MB |
| 0x3000_0000~3FFF_FFFF | - | 256 MB |
| 0x2000_0000~2FFF_FFFF | - | 256 MB |
| 0x0000_0000~1FFF_FFFF | Flash/ROM | 512 MB |

[See full datasheet](/atlas-linux/data/AT551.pdf)
