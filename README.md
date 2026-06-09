# ip-000004

Display name: APB4 GPIO Controller

UID: ip-000004

Family: gpio

Category: peripheral

Repository: git@github.com:openecos-projects/ip-000004.git

Upstream: https://github.com/oscc-ip/gpio

Upstream author/maintainer: Beijing Institute of Open Source Chip / OSCC-IP

Current baseline: source snapshot from the `20250627` tapeout project

License: MulanPSL-2.0, with selected files carrying Solderpad Hardware License 0.51 provenance notices

Status: candidate, silicon-proven source snapshot

This repository is managed as a child repository of `ip-catalog`.

## Summary

This IP is an APB4-based GPIO controller implemented in SystemVerilog. The
design supports up to 32 GPIO channels, input/output direction control, software
and alternate-function output selection, maskable input interrupts, and multiple
interrupt trigger modes.

The local repository contains a source mirror from the `20250627` tapeout
project for catalog evaluation. The current RTL baseline should be treated as
the tapeout project source snapshot rather than an automatically synchronized
upstream checkout.

## Layout

```text
rtl/       SystemVerilog RTL and required local common support modules
tb/        SystemVerilog testbench files
model/     GPIO simulation helper models
driver/    Minimal C software access example
docs/      Datasheet and provenance notes
reports/   Review, lint, simulation, or synthesis report summaries
```

## Top Level

The integration top module is:

```text
apb4_gpio
```

Top-level interfaces:

```text
apb4_if.slave apb4
gpio_if.dut   gpio
```

## Catalog Mapping

The corresponding catalog record is expected at:

```text
data/ip/peripheral/ip-000004.yaml
```

The local metadata source is:

```text
ip.yaml
```

## Review Notes

- Upstream repository: https://github.com/oscc-ip/gpio
- Upstream default branch observed locally: `main`
- Current source snapshot comes from the `20250627` tapeout project code.
- IP status is recorded as silicon-proven based on the provided tapeout project provenance.
- The RTL uses local common support modules copied into `rtl/`.
- No local passing simulation, lint, synthesis, coverage, or silicon validation report artifact has been added yet.
