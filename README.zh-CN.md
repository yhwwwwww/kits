# rsc Scoop bucket

[English — 主版本](README.md)

用于安装 [rsc](https://github.com/yhwwwwww/rsc) 的 Scoop 清单仓库。rsc 是用 Rust 独立实现的 Windows 包管理器。

## 安装

```powershell
scoop bucket add rsc https://github.com/yhwwwwww/scoop-bucket
scoop install rsc/rsc
```

清单支持 Windows x64，通过 SHA-256 校验发布程序。rsc 以单个可执行文件分发。

## 升级

```powershell
scoop update
scoop update rsc
```

## 维护

在 rsc 仓库的 **Actions → Release → Run workflow** 中编译并发布程序，然后自动更新 `bucket/rsc.json` 中的 Release 地址和准确校验值。工作流使用专用部署密钥，仅可写入这个 bucket。已发布版本不会覆盖。

本仓库只包含清单和文档，不包含 Scoop 实现代码。

## 许可证

[GNU GPL v3.0 only](LICENSE)。rsc 程序采用清单中声明的许可证。
