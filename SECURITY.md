# Security Policy

## Reporting a vulnerability

Email **chris.bouras@henos.io**. Do not open a public issue for a security
problem; a private report provides time to investigate and prepare a fix.

Include the canvas version and platform, the henosis engine version, relevant
configuration, reproduction steps, and the impact you observed. Do not include
credentials, private project data, or other secrets unless requested through a
secure channel.

## Supported versions

**henosis canvas** is a developer preview. Only the most recent published preview
is supported, and fixes are not necessarily backported to older previews.

## Local security model

The local canvas launcher binds canvas and its managed engine to loopback by
default. Do not expose either service directly to an untrusted network. Treat
henosis project credentials and any configured actions as access to the
underlying systems they represent.
