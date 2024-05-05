![Visitor](https://visitor-badge.laobi.icu/badge?page_id=KilianKegel.kiliankegel)

## logbook
* **2024-05-05**
  * add POST and EDK2-EMULATOR related bug fixes to  [Visual-TORO-C-LIBRARY-for-UEFI](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI?tab=readme-ov-file#20240505-v084-build-91) and [Toro C Library](https://github.com/KilianKegel/toro-C-Library?tab=readme-ov-file#20240505-v084-build-91)
* **2024-04-01**
  * improve [Visual-TSCSync-for-UEFI-Shell](https://github.com/KilianKegel/Visual-TSCSync-for-UEFI-Shell)
* **2024-03-24**
  * add SMBIOS support to [Visual-LIBWIN32-for-UEFI](https://github.com/KilianKegel/Visual-LIBWIN32-for-UEFI?tab=readme-ov-file#20240324)
* **2024-03-09**
  * add POSIX functions to  [Visual-TORO-C-LIBRARY-for-UEFI](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI?tab=readme-ov-file#20240309-v081-build-54)
* **2024-02-25**
  * update [Visual-UEFI-SHELL v1.5.0 Build 23](https://github.com/KilianKegel/Visual-UEFI-SHELL) to [edk2-stable202402](https://github.com/tianocore/edk2/releases/tag/edk2-stable202402)
  * introduce [EDK2-LIBC-AppDevelPORTABLE](https://github.com/KilianKegel/EDK2-LIBC-AppDevelPORTABLE)
* **2024-01-13**
  * introduce **portable** requirements for upcoming projects and updates [Howto-setup-a-UEFI-Development-PC](https://github.com/KilianKegel/Howto-setup-a-UEFI-Development-PC#preparation-for-upcoming-portable-projects)
  * improve to [Visual-TSCSync-for-UEFI-Shell – v1.2.3 Build 8](https://github.com/KilianKegel/Visual-TSCSync-for-UEFI-Shell#visual-tscsync-for-uefi-shell)
    * add 10000kHz digit rounding, e.g.
        * 1995379567 is rounded to 1995380000
        * 1995371234 is rounded to 1995370000
    * convert [Visual-ACPICA-for-UEFI-Shell](https://github.com/KilianKegel/Visual-ACPICA-for-UEFI-ShellPORTABLE) to [**PORTABLE MODEL**](https://github.com/KilianKegel/Visual-ACPICA-for-UEFI-ShellPORTABLE#20240113)
* **2024-01-07**
  * update [Visual-UEFI-SHELL](https://github.com/KilianKegel/Visual-UEFI-SHELL) – add [my-legacy-toolbox](https://github.com/tianocore/edk2-staging/blob/CdePkg/blogs/2021-11-14/README.md#my-legacy-toolbox) to internal PLUGIN command set
* **2024-01-06**
  * update [Visual-TSCSync-for-UEFI-Shell](https://github.com/KilianKegel/Visual-TSCSync-for-UEFI-Shell#visual-tscsync-for-uefi-shell)
* **2023-12-10**
  * update [Visual-TSCSync-for-UEFI-Shell](https://github.com/KilianKegel/Visual-TSCSync-for-UEFI-Shell#visual-tscsync-for-uefi-shell)
    * **NOTE**: Improvements apply only to recent INTEL(tm) platforms only. The particular CPUID leaf 0x15 and MSR **MSR_PLATFORM_INFO** are not available on AMD systems.
  * [Visual-UEFI-SHELL](https://github.com/KilianKegel/Visual-UEFI-SHELL#edk2-uefi-shell--visual-uefi-shell) update to recently released Intel Tianocore [edk2-stable202311](https://github.com/tianocore/edk2/releases/tag/edk2-stable202311)
    * add `DEFAULT_UEFI_DRIVE_NAMING` switch to **BOOTX64.INI**, to enable UEFI default drive naming **FS0:**, **FS1:**, **FS2:** ...
* **2023-11-19**
  * improve [Visual-TSCSync-for-UEFI-Shell](https://github.com/KilianKegel/Visual-TSCSync-for-UEFI-Shell)
  * improve [Toro C Library](https://github.com/KilianKegel/toro-C-Library#toro-c-library-formerly-known-as-torito-c-library)
  * update [CdePkg](https://github.com/KilianKegel/CdePkg) – C Development Environment Package for EDK2 and derived BIOS products
  * update [Visual ANSI C for UEFI Shell](https://github.com/KilianKegel/Visual-ANSI-C-for-UEFI-Shell#visual-ansi-c-for-uefi-shell)
* **2023-10-29**
  * update YOUTUBE appearance: https://www.youtube.com/@kiliankegel4598
  * update [Visual-UEFI-SHELL](https://github.com/KilianKegel/Visual-UEFI-SHELL) – Build UEFI SHELL binary from latest available EDK2 release tag
    * add **PCIView** plugin
    * https://www.youtube.com/watch?v=wXTQ_wsKwHw
  * update [Visual-TSCSync-for-UEFI-Shell](https://github.com/KilianKegel/Visual-TSCSync-for-UEFI-Shell#visual-tscsync-for-uefi-shell) – TSCSync - TimeStampCounter (TSC) synchronizer, analyze System Timer characteristics
    * improvement, *BETA RELEASE*
    * add **/METHOD:TIANO/ACPI/PIT** to select ACPI/PIT(i8254) or original *tianocore* calibration method
    * CONFIG Menu shows true timing values, instead of ACPI clock numbers
    * https://www.youtube.com/watch?v=I92emFEyTDI
* **2023-10-15**
  * Creation [Visual-TSCSync-for-UEFI-Shell](https://github.com/KilianKegel/Visual-TSCSync-for-UEFI-Shell#visual-tscsync-for-uefi-shell) – TSCSync - TimeStampCounter (TSC) synchronizer, analyze System Timer characteristics
  * update [Toro C Library](https://github.com/KilianKegel/toro-C-Library#toro-c-library-formerly-known-as-torito-c-library)
  * update all dependencies
* **2023-09-17**
  * Creation [Visual-UEFI-SHELL](https://github.com/KilianKegel/Visual-UEFI-SHELL) – Build UEFI SHELL binary from latest available EDK2 release tag
* **2023-09-16**
  * update [CdePkg](https://github.com/KilianKegel/CdePkg) – C Development Environment Package for EDK2 and derived BIOS products
  * update [Toro C Library](https://github.com/KilianKegel/toro-C-Library#toro-c-library-formerly-known-as-torito-c-library)
  * update [Visual ANSI C for UEFI Shell](https://github.com/KilianKegel/Visual-ANSI-C-for-UEFI-Shell#visual-ansi-c-for-uefi-shell)
* **2023-09-10**
  * update [CdePkg](https://github.com/KilianKegel/CdePkg) – C Development Environment Package for EDK2 and derived BIOS products
  * update [Visual-ACPICA-for-UEFI-Shell](https://github.com/KilianKegel/Visual-ACPICA-for-UEFI-Shell) – ACPI CA (ACPI component architecture) reference implementation for UEFI, using Visual Studio 2022 build environment


* **2023-09-09**
  * update [Toro C Library](https://github.com/KilianKegel/toro-C-Library#toro-c-library-formerly-known-as-torito-c-library)
  * update [Visual ANSI C for UEFI Shell](https://github.com/KilianKegel/Visual-ANSI-C-for-UEFI-Shell#visual-ansi-c-for-uefi-shell)

* **2023-08-26** [Visual-UEFI-SHELL](https://github.com/KilianKegel/Visual-UEFI-SHELL#edk2-uefi-shell--visual-uefi-shell) update to recently released Intel Tianocore [edk2-stable202308](https://github.com/tianocore/edk2/releases/tag/edk2-stable202308)
* **2023-05-01** Create new project: [Visual-UEFI-SHELL](https://github.com/KilianKegel/Visual-UEFI-SHELL#edk2-uefi-shell--visual-uefi-shell). Build UEFI SHELL binary from latest available EDK2 release tag

