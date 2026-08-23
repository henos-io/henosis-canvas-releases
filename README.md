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

Install Henosis Engine. From a Henosis project, run:

```bash
henosis canvas
```

The Engine resolves the latest release for your platform, verifies it against
`SHA256SUMS.txt`, caches it in your user application-data directory, starts the
local engine and Canvas, and opens Canvas in your browser. Pin a release with:

```bash
henosis canvas --canvas-version 0.1.0
```

For managed or offline environments, download and extract the platform archive,
then provide its launcher explicitly:

```bash
henosis canvas --canvas-path /path/to/henosis-canvas
```

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
