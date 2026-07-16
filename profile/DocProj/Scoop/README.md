[The Documentation Project](../README.md) ❭ Scoop

<div align="center">

### The Documentation Project

  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="../../.github/logo/dark/256x256.png">
    <source media="(prefers-color-scheme: light)" srcset="../../.github/logo/light/256x256.png">
    <img alt="Fallback image description" src="../../.github/logo/light/256x256.png">
  </picture>

# Scoop

</div>

> [!WARNING]
> Scoop must be installed on an NTFS-formatted drive.

| CONTENTS |
|----------|
| [Preparation](#preparation) |
| [Download installer](#download-installer) |
| [Install](#install) |
| [Add buckets](#add-buckets) |
| [Install applications](#install-applications) |

## Preparation

> This command must be run before using dvn, in an elevated PowerShell terminal (Administrator mode).

The first command makes your device allow running the installation and management scripts. This is necessary because Windows 10 client devices restrict execution of any PowerShell scripts by default.

`Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser`

## Download installer

Since we want to install Scoop to a custom location, we need to download the installer so we can run it with the appropriate parameters.

This command will download the installer to the root of the drive you want to install Scoop on:

`$@"irm get.scoop.sh -outfile '{drive}:\install.ps1'"`

For example:

`B:\Installers\Scoop\install.ps1`

## Install

> [!NOTE]
> The current version of dvn does not use global installs.

Install Scoop by running the installer:

`$@"{drive}:\install.ps1 -ScoopDir '{drive}:\Scoop\' -NoProxy"`

For example:

`.\install.ps1 -ScoopDir 'B:\Apps\Scoop' -ScoopGlobalDir 'B:\Apps\ScoopGlobal' -NoProxy`

### Add buckets

Make sure the required buckets are added::

`scoop bucket add extras`
`scoop bucket add sysinternals`

## Install applications

Search for application here: [Scoop](https://scoop.sh/)

* `scoop install extras/7zip`
* `scoop install extras/autohotkey`
* `scoop install extras/cpu-z`
* `scoop install extras/cryptomator`
* `scoop install extras/emeditor`
* `scoop install extras/firefox`
* `scoop install extras/gimp`
* `scoop install extras/gpu-z`
* `scoop install extras/lmstudio`
* `scoop install extras/notepadplusplus`
* `scoop install extras/sublime-text`
* `scoop install extras/treesize-free`
* `scoop install extras/vscode`
* `scoop install extras/wsl-ui`
* `scoop install sysinternals/sysinternals-suite`

<!--
* `scoop install extras/crystaldiskinfo`
* `scoop install extras/crystaldiskmark`
* `scoop install extras/discord`
* `scoop install extras/draw.io`
* `scoop install extras/etcher`
* `scoop install extras/ferdium`
* `scoop install extras/filezilla`
* `scoop install extras/gisto`
* `scoop install main/git`
* `scoop install extras/godot-mono`
* `scoop install extras/hwinfo`
* `scoop install extras/kitty`
* `scoop install extras/love`
* `scoop install extras/putty`
* `scoop install extras/rufus`
* `scoop install extras/signal`
* `scoop install extras/smartgit`
* `scoop install extras/telegram`
* `scoop install extras/vlc`
* `scoop install extras/windirstat`
* `scoop install extras/xampp`
    * suggests installing extras/vcredist2022
-->

<br>

***

[The Documentation Project](../README.md) ❭ Scoop

<sub>Last updated: 260716</sub>
