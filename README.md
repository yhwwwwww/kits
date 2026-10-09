# rsc Scoop bucket

[简体中文](README.zh-CN.md)

Scoop manifests for [rsc](https://github.com/yhwwwwww/rsc), an independent Windows package manager written in Rust.

## Install

```powershell
scoop bucket add rsc https://github.com/yhwwwwww/scoop-bucket
scoop install rsc/rsc
```

The manifest supports Windows x64 and verifies the release executable using SHA-256. rsc is distributed as a single executable.

## Update

```powershell
scoop update
scoop update rsc
```

## Maintenance

The rsc repository's **Actions → Release → Run workflow** builds and publishes the executable, then updates `bucket/rsc.json` with the exact release URL and checksum. A dedicated deploy key allows that workflow to write only to this bucket. Published versions are not overwritten.

This bucket contains manifests and documentation, with no Scoop implementation code.

## License

[GNU GPL v3.0 only](LICENSE). The rsc executable uses the license declared in its manifest.
