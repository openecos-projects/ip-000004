# Review Summary

## Status

`ip-000004` is a candidate child repository for the APB4 `gpio` IP.

## Source

- Source project: `20250627` tapeout project
- Upstream repository: `https://github.com/oscc-ip/gpio`
- Observed upstream commit: `9b578f0d4f9e0da5e7c852c3b2ebcb45c54a8d16`
- Mirror policy: source snapshot, no automated upstream synchronization

## Contents

- GPIO RTL under `rtl/`
- Required local common support under `rtl/`
- Testbench sources under `tb/`
- GPIO simulation helper models under `model/`
- Software access example under `driver/`
- Datasheet and provenance notes under `docs/`

## Open Items

- Attach tapeout validation evidence for the `20250627` project.
- Run and archive a reproducible simulation baseline.
- Run and archive lint results.
- Complete per-file license review for files carrying Solderpad provenance notices.
