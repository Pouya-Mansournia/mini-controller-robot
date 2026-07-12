# Roadmap

This roadmap is based only on repository evidence and current documentation gaps.

## Completed

- Altium project, schematic, PCB layout, output job, preview artifacts, and PDF export are committed.
- ATmega2560 firmware variants are committed.
- Existing debug build outputs are committed for the firmware variants.
- README, GitHub presentation notes, contribution guidance, and security notes are documented.

## In Progress

- Repository presentation cleanup and GitHub About metadata.

## Planned

- Add an explicit license file.
- Add validated board screenshots or renders for the README and GitHub social preview.
- Document the board pinout, connectors, power inputs, motor outputs, and current-sense channels.
- Document a verified flashing workflow, including programmer, fuse settings, and recovery steps.
- Regenerate and commit manufacturing outputs after ERC/DRC review.
- Separate source files from historical debug build outputs or move debug artifacts to releases.
- Add issue and pull-request templates.

## Requires Validation

- Physical board bring-up status.
- Motor driver current limits and safe operating envelope.
- Exact mechanical direction represented by serial commands `K` and `L`.
- Current telemetry scaling from raw ADC values to physical units.
