AppleALC Changelog
==================

#### v1.0.4
- Fixed a rare kernel panic due to uninitialised kern_proc
- Fixed a rare loading failure due to IOHDA value bruteforce necessity
- Added retry possibility for -alcpolicy
- Set -alcpolicy mode the default mode
- Added ALC269VC for Lenovo V850 codec support (by Ar4erR07)
- Added ALC282 DSP features and config improvements (by savvamitrofanov)
- Added ALC663, layout-id 28 codec support (by m-dudarev)
- Added ALC887-VD for Z97 codec support (by John998)

#### v1.0.3
- Fixed AAPL,ig-platform-id naming
- Added preliminary start modes support
- Added TrustedBSD start via -alcpolicy and IOService::start via -alciokit arguments
- Allowed kext patches with 0 count replacing all entries (use this with a reason)
- Fixed ALC270 regressions
- Added ALC889, layout-id 12 codec support (by Sergey_Galan)
- Added ALC887-VD, layout 99 codec support (by Constanta)
- Removed unnecessary NVIDIA GT240 HDMI patches

#### v1.0.2
- Added Controller.plist with controller-specific patches
- Added Intel X99 and Intel HD4600 controller patches
- Reverted device-id comparison code, it was redundant
- Added prelinkedkernel reading (used exclusively in OS X Installer/Recovery HD)
- Added AppleIntelFramebufferAzul patches to fix HD4600 audio
- Added ALC269 10.9.x/10.10.x patches (by Andrey1970)
- Added ALC269 for Asus K53SJ (by alex1960)
- Added ALC270 codec support (by m-dudarev)
- Added ALC270 for Asus K56CB (by m-dudarev)
- Added ALC668 for Asus N750Jk (by alex1960)
- Added ALC885 (by alex1960)
- Added NVIDIA GT240 HDMI patches (by Vandroiy)
- Added Intel HD4000 patches (by Andrey1970)

#### v1.0.1
- boot-args presence is now optional
- Platforms must conform to layout-id from now on
- Workaround a race-condition kernel panic when accessing current_thread credential
- Fixed a kernel panic when kaslr is disabled
- Renamed control boot arguments to -alcdbg and -alcoff
- Added optional device-id comparison to patch and file matching
- Added PinConfs plugin injecting pin configurations
- Added AD1988B codec support (by Rodion)
- Added ALC269VC (Lenovo Z580) codec support (by John)
- Added ALC269 (Acer Aspire) codec support (by Andrey1970)
- Added ALC282 codec support (by S.Mitrofanov)
- Added ALC887 codec support (by x-tropic)
- Added ALC888 codec support (by Vandroiy)
- Added ALC889 codec support (by Ukr55)
- Added ALC892 codec support (by FredWst, m-dudarev)
- Added ALC898 codec support (by Andrey1970)
- Added CX20590 codec support (by usr-sse2)

#### v1.0.0
- Initial release
