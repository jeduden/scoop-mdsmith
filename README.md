# scoop-mdsmith

A [Scoop](https://scoop.sh) bucket for [mdsmith](https://github.com/jeduden/mdsmith),
a fast Markdown linter and formatter. The bucket serves the official Windows
binary (`mdsmith-windows-amd64.exe`) from each upstream GitHub release, pinned to
the SHA-256 checksum that Scoop verifies on install. The manifest is not
hand-maintained: an excavator workflow re-runs Scoop's autoupdate on a daily
schedule, on manual dispatch, and immediately whenever mdsmith publishes a new
release, so the pinned version and hash always track the latest upstream tag.

## Install

```sh
scoop bucket add mdsmith https://github.com/jeduden/scoop-mdsmith
scoop install mdsmith
```

After install, the `mdsmith` command is on your PATH:

```sh
mdsmith --version
```
