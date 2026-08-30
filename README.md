[![](https://img.shields.io/nuget/v/soenneker.libraries.ffmpeg.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libraries.ffmpeg/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libraries.ffmpeg/build-and-test.yml?style=for-the-badge)](https://github.com/soenneker/soenneker.libraries.ffmpeg/actions/workflows/build-and-test.yml)
[![](https://img.shields.io/nuget/dt/soenneker.libraries.ffmpeg.svg?style=for-the-badge)](https://www.nuget.org/packages/soenneker.libraries.ffmpeg/)
[![](https://img.shields.io/github/actions/workflow/status/soenneker/soenneker.libraries.ffmpeg/codeql.yml?label=CodeQL&style=for-the-badge)](https://github.com/soenneker/soenneker.libraries.ffmpeg/actions/workflows/codeql.yml)

# Soenneker.Libraries.FFmpeg

The FFmpeg Windows executable packaged as a .NET content asset.

## Install

```bash
dotnet add package Soenneker.Libraries.FFmpeg
```

The package copies the executable beneath the application output directory:

```text
Resources/ffmpeg.exe
```

Resolve it without depending on the process working directory:

```csharp
string ffmpeg = Path.Combine(AppContext.BaseDirectory, "Resources", "ffmpeg.exe");
```

This package supplies the Windows executable but does not start or manage FFmpeg. Use `ProcessStartInfo.ArgumentList` when building commands from variable input so paths and values remain separate arguments.
