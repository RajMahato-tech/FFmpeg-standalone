# FFmpeg standalone for Windows

This repository contains a prebuilt, portable 64-bit Windows FFmpeg distribution, including command-line tools, shared libraries, headers, import libraries, and HTML documentation. No installer is required.

## Build information

- **FFmpeg version:** `N-119294-g7684243fbe-20250417`
- **Upstream revision:** `7684243fbe`
- **Build date:** 2025-04-17
- **Target:** x86_64 Windows (MinGW-w64)
- **Compiler:** GCC 14.2.0
- **Build configuration:** shared libraries enabled; GPL and version 3 enabled

The binaries identify their complete configuration and library versions with:

```powershell
.\bin\ffmpeg.exe -version
```

## Contents

- `bin/` — `ffmpeg.exe`, `ffprobe.exe`, `ffplay.exe`, and their DLL dependencies
- `include/` — FFmpeg development headers
- `lib/` — import libraries, module definition files, and pkg-config files
- `doc/` — FFmpeg HTML documentation
- `LICENSE.txt` — GPL version 3 license text

## Requirements

## Plug and play

Download and extract the package, then run `bin\ffmpeg.exe`, `bin\ffprobe.exe`, or `bin\ffplay.exe`. You can copy the extracted folder wherever you need it; keep the DLL files in `bin/` beside the executables. To use FFmpeg from another application, point the application to `bin\ffmpeg.exe`, or add the `bin/` directory to your `PATH`.

## Licensing

This build was configured with `--enable-gpl` and `--enable-version3`. Review `LICENSE.txt`, the FFmpeg licensing information, and the licenses and source-code requirements for all bundled third-party libraries before redistributing this build.
