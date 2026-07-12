# Security Policy

## Scope

This repository contains embedded controller hardware and firmware. It does not currently include a network service, web application, cloud backend, authentication layer, firmware signing flow, or secure boot process.

## Reporting a Vulnerability

Please report suspected security issues through GitHub Issues unless a private reporting channel is later added to the repository.

Useful reports include:

- Unsafe motor-control behavior reachable through the serial command interface.
- Firmware behavior that can damage the board, motors, batteries, or connected equipment.
- Incorrect power, fuse, flashing, or bench-test guidance.
- Accidental exposure of credentials, private paths, or sensitive design information.

## Known Security Boundaries

- USART0 commands are unauthenticated.
- Motor outputs can be energized by single-byte serial commands.
- The repository does not document secure firmware update, signing, rollback, or access control.
- Hardware use should begin with a current-limited bench setup before connecting full loads.
