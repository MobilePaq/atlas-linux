---
layout: default
title: Firmware details
nav_order: 3
description: "Firmware details for Atlas-linux"
---

# Firmware details

## Files contained in OEM factory update (Explay **PN-975 Atlas V**)

| File | Size | Description | Contents | Download |
| ---- | ---- | ----------- | -------- | -------- |
| chain.bin | 2KB | Instructions for bootloader | Signature "B000FF"(ASCII), 4 bytes and then filename | [PN-975](/atlas-linux/data/PN975/chain.bin) |
| chain.lst | 1KB | Instructions for bootloader | List of firmware files, "+" before one that will be booted | [PN-975](/atlas-linux/data/PN975/chain.lst) |
| NK.bin | 30-32MB | Main firmware image | Signature "B000FF"(ASCII), then WinCE data | [PN-975](/atlas-linux/data/PN975/NK.bin) |
| TINYNK.bin | 4-6MB | Tiny Kernel/Updater? | Signature "B000FF"(ASCII), then WinCE data | [PN-975](/atlas-linux/data/PN975/TINYNK.bin) |
| LHApp.rar | 6MB | Main launcher APP for CE | ??? | [PN-975](/atlas-linux/data/PN975/LHApp.bin) |
| format.cfg | 0 | Flag file to erase all user data | Empty | *Why would you need an empty file?* |
