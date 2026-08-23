# Henosis Canvas Developer Preview

This repository contains binary releases of Henosis Canvas. The Canvas source
code is maintained separately and is not published here.

Canvas is the local visual workspace for the open-source
[Henosis Engine](https://github.com/henos-io/henosis). It runs on your machine,
connects to a Henosis project, and exposes the Canvas and engine MCP endpoints
on loopback interfaces.

## Download

Download the archive for your platform from
[Releases](https://github.com/henos-io/henosis-canvas-releases/releases):

- Windows x64
- macOS arm64

Do not use GitHub's automatically generated **Source code** archives. They
contain only this release repository's documentation, not Henosis Canvas.

Verify the archive against `SHA256SUMS.txt` before extracting it.

## Run

Install Henosis Engine, extract the Canvas archive, and add its `bin` directory
to your `PATH`. From a Henosis project, run:

```bash
henosis canvas
```

The command starts the local engine and Canvas, opens Canvas in your browser,
and stops both processes when the launcher exits.

You can also invoke the extracted launcher directly:

```bash
henosis-canvas --project /path/to/project
```

On Windows, the launcher is `henosis-canvas.cmd`.

## Preview status

This is an early developer preview intended for evaluation, not production
use. See [PREVIEW_TERMS.md](PREVIEW_TERMS.md) before downloading or using it.

Security issues should be reported privately as described in
[SECURITY.md](SECURITY.md).
