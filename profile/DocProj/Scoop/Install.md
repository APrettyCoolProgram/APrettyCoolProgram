<!-- 260505 -->

[The APCP Documentation Project](../README.md) ❱ Scoop ❱ Scoop Overview

***

<div align="center">

### The APCP Documentation Project

  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="../../.github/logo/dark/256x256.png">
    <source media="(prefers-color-scheme: light)" srcset="../../.github/logo/light/256x256.png">
    <img alt="Fallback image description" src="../../.github/logo/light/256x256.png">
  </picture>

# Install Scoop

</div>

> [!WARNING]
> Scoop must be installed on an NTFS-formatted drive.

[Scoop](https://scoop.sh/)

## Scoop prerequisites

> This command must be run before using dvn, in an elevated PowerShell terminal (Administrator mode).

The first command makes your device allow running the installation and management scripts. This is necessary because Windows 10 client devices restrict execution of any PowerShell scripts by default.

`Set-ExecutionPolicy -ExecutionPolicy RemoteSigned -Scope CurrentUser`

## Download the Scoop installer

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

<br>

***

[The APCP Documentation Project](../README.md) ❱ Scoop ❱ Scoop Overview