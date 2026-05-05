<!-- 260505 -->

[The APCP Documentation Project](../README.md) ❱ Scoop ❱ Scoop Overview

***

<div align="center">

### The APCP Documentation Project

  <picture>
    <source media="(prefers-color-scheme: dark)" srcset=".github/repository/logo/apcp-logo-dark-256x256.png">
    <source media="(prefers-color-scheme: light)" srcset=".github/repository/logo/apcp-logo-light-256x256.png">
    <img alt="Fallback image description" src="../.github/repository/logo/apcp-logo-light-256x256.png">
  </picture>

# Scoop Overview

</div>

> [!WARNING]
> Scoop must be installed on an NTFS-formatted drive.

[Scoop](https://scoop.sh/)

## Install Scoop

### Scoop prerequisites

> This command must be run before using dvn, in an elevated PowerShell terminal (Administrator mode).

The first command makes your device allow running the installation and management scripts. This is necessary because Windows 10 client devices restrict execution of any PowerShell scripts by default.

`Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser`

### Download the Scoop installer

Since we want to install Scoop to a custom location, we need to download the installer so we can run it with the appropriate parameters.

This command will download the installer to the root of the drive you want to install Scoop on:

`$@"irm get.scoop.sh -outfile '{drive}:\install.ps1'"`

For example:

`B:\Installers\Scoop\install.ps1`

### Install

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

## Install Scoop applications

* `scoop install extras/audacity`
* `scoop install extras/cryptomator`
* `scoop install extras/etcher`
* `scoop install extras/rufus`
* `scoop install extras/smartgit`
* `scoop install extras/vscode`
* `scoop install extras/yumi-exfat`
* `scoop install sysinternals/sysinternals-suite`


  
<!--
* `scoop install extras/autohotkey`
* `scoop install extras/cpu-z`
* `scoop install extras/crystaldiskinfo`
* `scoop install extras/crystaldiskmark`
* `scoop install dbeaver`
* `scoop install extras/discord`
* `scoop install extras/draw.io`
* `scoop install extras/etcher`
* `scoop install extras/ferdium`
* `scoop install extras/filezilla`
* `scoop install extras/firefox`
* `scoop install extras/gimp`
* `scoop install extras/gisto`
* `scoop install main/git`
* `scoop install extras/godot-mono`
* `scoop install extras/gpu-z`
* `scoop install extras/hwinfo`
* `scoop install extras/kitty`
* `scoop install extras/love`
* `scoop install extras/notepadplusplus`
* `scoop install extras/putty`
* `scoop install extras/rufus`
* `scoop install extras/signal`
* `scoop install extras/smartgit`
* `scoop install extras/sublime-text`
* `scoop install sysinternals/sysinternals-suite`
* `scoop install extras/telegram`
* `scoop install extras/vlc`
* `scoop install extras/windirstat`
* `scoop install extras/xampp`
    * suggests installing extras/vcredist2022
-->

<br>

***

[The APCP Documentation Project](../README.md) ❱ Scoop ❱ Scoop Overview
