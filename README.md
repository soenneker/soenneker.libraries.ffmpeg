[![](https://img.shields.io/nuget/v/soenneker.libraries.ffmpeg.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libraries.ffmpeg/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libraries.ffmpeg/build-and-test.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libraries.ffmpeg/actions/workflows/build-and-test.yml)
[![](https://img.shields.io/nuget/dt/soenneker.libraries.ffmpeg.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libraries.ffmpeg/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libraries.ffmpeg/codeql.yml?label=CodeQL&style=for-the-badge)](https://github.com/soenneker/soenneker.libraries.ffmpeg/actions/workflows/codeql.yml)

# Soenneker.Libraries.FFmpeg

Simply adds the FFmpeg Windows executable, updated daily (if available).

## Install

```bash
dotnet add package Soenneker.Libraries.FFmpeg
```

## What it provides

- Simply adds the FFmpeg Windows executable, updated daily (if available).
- The file is copied to the output directory, and located at the relative path: `Resources\ffmpeg.exe`.

## How to use it

After installation, resolve the packaged file from the output-relative path above. The package deploys the asset but does not invoke it for you.
