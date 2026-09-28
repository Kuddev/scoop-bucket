# Pebrel Scoop bucket

Windows x64 and ARM64 packages for [Pebrel](https://github.com/Kuddev/pebrel).

Pebrel 的 Scoop 安装源，提供 Windows x64 和 ARM64 应用包。

## Install / 安装

Install [Scoop](https://scoop.sh/) first, then run in a regular PowerShell session:

先安装 Scoop，再在普通 PowerShell 窗口中执行：

```powershell
scoop bucket add pebrel https://github.com/Kuddev/scoop-bucket
scoop install pebrel/pebrel
```

Launch Pebrel from the Start menu or run `pebrel` in your terminal.

安装后可从开始菜单启动，或在终端执行 `pebrel`。

## Update / 更新

```powershell
scoop update
scoop update pebrel
```

Use Scoop to update this installation. A new application release becomes
available here after its manifest is updated in this bucket.

通过 Scoop 更新此安装；新版本的安装清单更新到本仓库后，即可使用上述命令升级。

## Uninstall / 卸载

```powershell
scoop uninstall pebrel
```

The manifest does not remove application settings stored outside the installation
directory. To remove the bucket separately, run `scoop bucket rm pebrel`.

卸载不会由本清单删除安装目录外的应用设置。若要另外移除安装源，可执行
`scoop bucket rm pebrel`。

## Package source / 软件来源

- Downloads come from the project's official [GitHub Releases](https://github.com/Kuddev/pebrel/releases).
- Scoop verifies the SHA256 digest declared in `bucket/pebrel.json`.
- The complete portable package, including native console helpers and licenses,
  is preserved; no separate installer is executed.
- Application license: GPL-3.0-or-later; bundled components retain their own notices.

应用包直接来自项目的 GitHub Releases，由 Scoop 校验 SHA256；保留完整便携包、
控制台辅助文件和许可证，不运行另外的安装器。

Report installation-manifest issues in this repository. Report application issues
in [Kuddev/pebrel](https://github.com/Kuddev/pebrel/issues).
