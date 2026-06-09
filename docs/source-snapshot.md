# Source Snapshot

This repository packages the `gpio` IP as `ip-000004` for catalog review.

The source baseline is the `20250627` tapeout project code. The RTL in this
repository should be treated as a project source snapshot rather than an
automatically synchronized mirror of upstream `main`.

Observed upstream context from the local `new_ip/gpio` checkout:

- Repository: `https://github.com/oscc-ip/gpio`
- Branch: `main`
- Commit: `9b578f0d4f9e0da5e7c852c3b2ebcb45c54a8d16`
- Commit date: `2024-09-09 18:40:22 +0800`
- Commit subject: `feat: use iocfg cfg to rewrite alt in io logic`

The packaged RTL also includes the local common support modules required to
compile and simulate the IP standalone for catalog review.
