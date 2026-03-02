# S7 PPI USB Analyzer

Custom Wireshark Lua dissector for Siemens S7-200 (PPI over USB).

![Version](https://img.shields.io/badge/version-1.0-blue)
![Status](https://img.shields.io/badge/status-stable-brightgreen)
![License](https://img.shields.io/badge/license-MIT-green)

## Architecture

USB (Bulk Transfer)
  ↓
PPI Frame Reassembly
  ↓
S7 Layer Parser
  ↓
IDS Level 1 (Passive Detection)
  ↓
Statistics Engine

## Limitations

- Designed for Siemens S7-200 over PPI only
- Bound to USB VID 0908 / PID 0004
- IDS is passive (detection only, no blocking)
- Not performance-optimized (Lua-based)

- 
