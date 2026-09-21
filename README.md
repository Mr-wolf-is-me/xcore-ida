# xCore IDA Support package

Native XMOS xCORE/XS3 analysis for IDA Pro 8.4.

If you work with XMOS firmware, this package gives IDA the architecture knowledge it needs to
turn raw xCORE ELF files into useful disassembly: instruction families, registers, operands,
branches, calls, memory references, and processor-specific behavior.

## What you get

- xCORE/XS3 processor support for IDA Pro
- CSV-driven instruction definitions based on the XS3 architecture manual
- Register-aware operands, including stack, resource, CP, DP, and PC-relative references
- Control-flow analysis for branches, calls, returns, and switch-style jump tables
- Constant-pool resolution for CP-based instructions
- xCORE ABI calling-convention support
- DWARF prototype importing through the XMOS XTC toolchain
- ISA documentation lookup from the disassembly view
- Dynamic xCORE debugging with IDA through xgdbserver
- Debugger tools and ready-to-run command scripts
- IDAPython definitions for xCORE registers and instruction identifiers

## Quick start

1. Extract the deployment package into writable folder.
2. Run `cmd\xcore_ida.cmd` to launch IDA with the deployment configured.
3. Open an xCORE/XS3 ELF file in IDA Pro 8.4.
4. For debugging, configure the included command scripts with the IDA path, XMOS XTC path, and XE file.

The package is designed to work as a self-contained IDA user directory and does not modify the
IDA installation.

## Terms of use

By downloading, installing, or using this package, you accept the terms in
[LICENSE.md](LICENSE.md).

## Documentation

The XS3 ISA PDF is intentionally not bundled. Obtain it separately if you want instruction
documentation lookup, then place it where the documentation configuration expects it.

Supported IDA version: 8.4

Author: [mr.wolf.is.me@gmail.com](mailto:mr.wolf.is.me+xcore_ida@gmail.com)
