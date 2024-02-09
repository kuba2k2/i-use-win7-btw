# i use win7 btw

Windows 7 Fan-Made Survival Guide

## Introduction

This is a list of applications, games, frameworks, updates, patches, etc. compatible with the Windows 7 operating system.

Software listed on this page can either be compatible with vanilla Windows 7 or it might require adding missing DLLs
or other patches, to either the mentioned software or the entire OS.

### Help! XYZ is missing, what can I do?

There's no way I can possibly list all software ever made - **but you can help!**

If you find something is missing - be it your favorite game, a web browser, or a magic solution to run all modern apps -
I'll be very happy to accept your contribution to this list.

Simply press **Edit file**, change what you need and press **Commit changes**. Then, create a pull request (PR) back
to this repository.

### What kind of software should I add?

Basically, everything that you're using daily. There are no strict rules - even software **incompatible** with Windows 7
can be added - who knows, maybe it will be patched one day.

That being said, this list is mostly for **maintained, still developed software**. So try not to add programs that
haven't been updated for the past 15 years.

I'm also interested in any Windows patches or modifications! If you ported some software from a different version of
Windows, feel free to add it to the list too.

---

## Updates, patches & tweaks

Essentials:

- [BypassESU](https://forums.mydigitallife.net/threads/bypass-windows-7-extended-security-updates-eligibility.80606/) (login required) - A project to install Extended Security Updates for Windows 7 and Server 2008 R2
- [wufuc](https://github.com/chipsi007/wufuc) - Disables the "Unsupported Hardware" message in Windows Update
- [Windows 7 ESU Patching](https://hackandpwn.com/windows-7-esu-patching/) by [HackAndPwn](https://hackandpwn.com/) - comprehensive list of official Windows updates and their meaning for `the most up-to-date installation possible`

Tweaks:

- [7+ Taskbar Tweaker](https://ramensoftware.com/7-taskbar-tweaker) - Configure various aspects of the Windows taskbar
- [Winaero Tweaker](https://winaerotweaker.com/) - The ultimate all-in-one app for tuning Windows 11, Windows 10, Windows 8, and Windows 7
- [AccentColorizer](https://github.com/krlvm/AccentColorizer) - Colorize Windows with accent color of your choice

Ported software/user modifications:

- [SnippingToolEx](https://github.com/vxiiduu/SnippingToolEx) - Win10 snipping tool ported to Windows Vista and 7

Patches:

- [VxKex](https://github.com/vxiiduu/VxKex) - Windows 7 API Extensions by [vxiiduu](https://github.com/vxiiduu)
- [[WIP] Windows 7 Extended Kernel](https://msfn.org/board/topic/184971-wip-windows-7-extended-kernel/) by [dotexe1337](https://github.com/dotexe1337)
- [api-ms-win-core-path-HACK](https://github.com/nalexandru/api-ms-win-core-path-HACK) - Implementation of api-ms-win-core-path-l1-1-0.dll for Windows 7 based on Wine code
- [API-MS-WIN_XP](https://github.com/Blaukovitch/API-MS-WIN_XP) - Microsoft API libs Windows 11/10/8/ to Windows XP

Other repositories:

- [Windows 7 & Thorium](https://thorium.rocks/win7) - Unofficial builds of software based on the [Thorium browser](https://github.com/Alex313031/thorium-win7) (Chromium fork), also some other patched software
- [Compatibility List](https://thorium.rocks/misc/win7_compat_list.html) by the same author ([Alex313031](https://github.com/Alex313031)). Contains download links.

---

## Compatibility list

Meaning of used terms and symbols.

Versions:

- **Official** - last version officially supported on W7.
	- `Supported` if still officially supported
	- `None` if it was never supported
	- `Dropped` if support was dropped with no clear info about latest working version
	- `Broken` if support was dropped without announcement, i.e. it "just stopped working"
- **Tested** - latest **official** version verified to work on W7
- **Compatible** - **unmodified** version that "just works" on **vanilla** W7, despite dropping official support (usually empty)
- **Patched** - version that works after applying patches (i.e. DLLs) to either the software or the OS (i.e. extended kernels)

Fields you're not sure about should be left empty. Same if there are no patched versions.

Symbols:

- ❗ - having some issues
- ❓ - untested
- 🇵 - with patching either source code or binaries (include links below)
- 🇩 - with adding missing DLLs manually
- 🇻 - with VxKex
- 🇪 - with Windows 7 Extended Kernel

## Languages/frameworks

Programming languages, libraries and frameworks.

Name     | Official | Tested  | Compatible | Patched
---------|----------|---------|------------|----------
Electron | 22       |         |            |
Go       | 1.20     |         | 1.21.4     |
Node.js  | 12.22.12 | 16.18.1 | 19.9.0     |
Python   | 3.8.18   |         |            | 🇵 3.12.2

- [PythonWin7](https://github.com/adang1345/PythonWin7)
- Node.js: [use .zip binaries](https://nodejs.org/en/about/previous-releases), v20.x doesn't work anymore. Installers may work with `NODE_SKIP_PLATFORM_CHECK=1`

## Applications

### Web Browsers

Name                         | Official       | Tested         | Compatible | Patched
-----------------------------|----------------|----------------|------------|--------
Firefox                      | 115 ESR        |                |            |
Firefox Developer Edition    | 115            | 115.0b9        |            |
Google Chrome                | 109            | 109.0.5414.120 |            |
Microsoft Edge               | 109            | 109.0.1518.140 |            |
Supermium (Chromium fork)    | 121.0.6167.81  |                |            |
Thorium (Chromium fork)      | 109.0.5414.173 |                |            |
Thorium-Win7 (Chromium fork) | 119.0.6045.214 |                |            |

- [Google Chrome](https://edgedl.me.gvt1.com/edgedl/release2/10/windows-8/googlechromestandaloneenterprise64.msi) - latest MSI
- [Supermium](https://github.com/win32ss/supermium/releases)
- [Thorium](https://github.com/Alex313031/thorium-win7)

### Multimedia

Name | Official | Tested | Compatible | Patched
-----|----------|--------|------------|--------
     |          |        |            |

### Social/communication

Name    | Official | Tested   | Compatible | Patched
--------|----------|----------|------------|----------
Discord | Dropped  | 1.0.9032 |            |
Caprine | Broken   | 2.57.1   |            | 🇵 2.59.3

- [Caprine-ng](https://github.com/Alex313031/caprine-ng)

### Office

Name                | Official  | Tested  | Compatible | Patched
--------------------|-----------|---------|------------|--------
Mozilla Thunderbird | Supported | 115.7.0 |            |

### Graphics/design/CAD

Name | Official | Tested | Compatible | Patched
-----|----------|--------|------------|--------
     |          |        |            |

### Developer tools/IDEs

Name              | Official  | Tested   | Compatible | Patched
------------------|-----------|----------|------------|----------
Git               | Supported | 2.40.1   |            |
GitKraken         | Dropped   | 9.11.0   |            |
Insomnia          | Broken    | 2022.6.0 |            |
VS Code/VS Codium | 1.70.3    | 1.70.3   |            | 🇵 1.86.0
WakaTime          | Broken    |          |            |

- [VSCodium Fork with Optimizations](https://github.com/Alex313031/codium)

### Utilities

Name       | Official  | Tested | Compatible | Patched
-----------|-----------|--------|------------|--------
Chocolatey | Supported | 2.2.2  |            |
Fing       |           | 2.10.0 |            |
Rufus      | 3.22      | 3.11   |            |
Syncthing  | Broken    | 1.27.0 |            |

### Other

Name | Official | Tested | Compatible | Patched
-----|----------|--------|------------|--------
     |          |        |            |

## Games

### Launchers

Name  | Official | Tested     | Compatible | Patched
------|----------|------------|------------|--------
Steam | Dropped  | 1705108172 |            |

### Games

Name | Official | Tested | Compatible | Patched
-----|----------|--------|------------|--------
     |          |        |            |
