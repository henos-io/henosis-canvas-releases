# Security Policy

## Reporting a vulnerability

Email **chris.bouras@henos.io**. Do not open a public issue for a security
problem; a private report provides time to investigate and prepare a fix.

Include the Canvas version and platform, the Henosis Engine version, relevant
configuration, reproduction steps, and the impact you observed. Do not include
credentials, private project data, or other secrets unless requested through a
secure channel.

## Supported versions

Henosis Canvas is a developer preview. Only the most recent published preview
is supported, and fixes are not necessarily backported to older previews.

## Local security model

The local Canvas launcher binds Canvas and its managed engine to loopback by
default. Do not expose either service directly to an untrusted network. Treat
Henosis project credentials and any configured actions as access to the
underlying systems they represent.
