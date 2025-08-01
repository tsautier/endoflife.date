---
title: Deno
addedAt: 2025-02-16
category: framework
tags: javascript-runtime
iconSlug: deno
permalink: /deno
versionCommand: deno --version
releasePolicyLink: https://docs.deno.com/runtime/fundamentals/stability_and_releases/
changelogTemplate: https://github.com/denoland/deno/releases/tag/v__LATEST__

identifiers:
-   purl: pkg:docker/denoland/deno
-   purl: pkg:github/denoland/deno
-   repology: deno

auto:
  methods:
  -   git: https://github.com/denoland/deno.git

# non-LTS : eol(x) = releaseDate(x+1)
# LTS : eol(x) = releaseDate(x+1) + 5 months
# LTS releases are listed on https://docs.deno.com/runtime/fundamentals/stability_and_releases/.
releases:
-   releaseCycle: "2.4"
    releaseDate: 2025-07-01
    lts: 2025-11-01
    eol: 2026-04-30
    latest: "2.4.3"
    latestReleaseDate: 2025-07-30

-   releaseCycle: "2.3"
    releaseDate: 2025-04-30
    eol: 2025-07-01
    latest: "2.3.7"
    latestReleaseDate: 2025-06-23

-   releaseCycle: "2.2"
    releaseDate: 2025-02-18
    lts: 2025-05-01
    eol: 2025-10-31
    latest: "2.2.14"
    latestReleaseDate: 2025-07-16

-   releaseCycle: "2.1"
    releaseDate: 2024-11-21
    lts: 2025-02-01
    eol: 2025-04-30
    latest: "2.1.13"
    latestReleaseDate: 2025-05-13

-   releaseCycle: "2.0"
    releaseDate: 2024-10-08
    eol: 2024-11-21
    latest: "2.0.6"
    latestReleaseDate: 2024-11-10

-   releaseCycle: "1"
    releaseDate: 2020-04-13
    eol: 2024-10-09
    latest: "1.46.3"
    latestReleaseDate: 2024-09-04

---

> [Deno](https://deno.com) is a JavaScript, TypeScript, and WebAssembly runtime with
> secure defaults and a great developer experience. It's built on V8, Rust, and Tokio.

Deno follows [SemVer](https://semver.org/). New minor releases are made monthly and
are supported with bug and security fixes until the next minor release.
Every six months a minor version is promoted to LTS and is supported with critical
bug and security fixes for an additional 5 months.

Deno maintainers are committed to maintaining a stable standard library API (`Deno`
namespace) from version `1.0.0` onward.
