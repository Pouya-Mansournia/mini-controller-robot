# Contributing

Thank you for helping improve Mini Controller Robot. This repository contains both hardware design files and embedded firmware, so useful contributions should be specific about which layer changed and how it was checked.

## Before You Start

- Open an issue for larger hardware, firmware, or documentation changes.
- Confirm whether your change affects the Altium board design, the ATmega2560 firmware, or both.
- Avoid mixing unrelated cleanup with functional changes.

## Hardware Changes

For changes to `Mini Control Board.PrjPcb`, `Mini Control Board.SchDoc`, or `Mini Control Board.PcbDoc`:

- Describe the electrical or mechanical reason for the change.
- Run Altium ERC/DRC where possible.
- Regenerate output files only when they are intentionally part of the change.
- Include notes for any connector, motor driver, power, or current-sense behavior that firmware depends on.

## Firmware Changes

For changes under `MICRO TEST Version1 Source Code/`:

- State which firmware variant changed: `PEM1`, `PEM2`, or `Version1`.
- Rebuild the related CodeVisionAVR project when possible.
- Note compiler warnings and whether they are new or existing.
- Document any serial command, baud rate, pin mapping, timer, PWM, ADC, or fuse assumption changes.

## Pull Request Checklist

- The README is updated if user-visible behavior changed.
- New commands, board assumptions, or flashing steps are documented.
- Generated files are included only when they are intentional.
- Manual hardware or bench-test notes are included for motor-control changes.
- No secrets, local machine paths, or private credentials are added.
