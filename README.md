# henosis canvas Developer Preview

This repository contains binary releases of **henosis canvas**. The canvas source
code is maintained separately and is not published here.

**henosis canvas** is the local visual workspace for the open-source
[henosis engine](https://github.com/henos-io/henosis). It runs on your machine,
connects to a henosis project, and exposes the canvas and engine MCP endpoints
on loopback interfaces.

## Download

Most users do not need to download canvas manually. Running `henosis canvas`
causes henosis engine to download, verify and cache the latest compatible
release automatically.

Download an archive explicitly only when working offline or using an
organisation-managed binary. Select your platform from
[Releases](https://github.com/henos-io/henosis-canvas-releases/releases):

- Windows x64
- macOS arm64

Do not use GitHub's automatically generated **Source code** archives. They
contain only this release repository's documentation, not **henosis canvas**.

Verify a manually downloaded archive against `SHA256SUMS.txt`, extract it, then
pass its launcher to `henosis canvas --canvas-path` as shown below.

## Run

Install henosis engine. From a henosis project, run:

```bash
henosis canvas
```

The engine resolves the latest release for your platform, verifies it against
`SHA256SUMS.txt`, caches it in your user application-data directory, starts the
local engine and canvas, and opens canvas in your browser. Pin a release with:

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
