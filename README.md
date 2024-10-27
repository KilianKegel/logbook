![Visitor](https://visitor-badge.laobi.icu/badge?page_id=KilianKegel.kiliankegel)

## logbook
* **2024-10-27**
   * update [Visual-ACPICA-for_UEFI](https://github.com/KilianKegel/Visual-ACPICA-for-UEFI-ShellPORTABLE?tab=readme-ov-file#visual-acpica-for-uefi-shell) to [**ACPI CA v20240927**](https://www.intel.com/content/www/us/en/developer/topic-technology/open/acpica/download.html)
   * integrate **ACPI CA** tools into [**Visual-UEFI-Shell**](https://github.com/KilianKegel/Visual-UEFI-SHELL?tab=readme-ov-file#edk2-uefi-shell--toro-uefi-shell):
    * `AslCompiler` 
	  * `AcpiDump`
	  * `AcpiBin`
	  * `AcpiExec`
	  * `AcpiHelp`
	  * `AcpiSrc`
	  * `AcpiXtract` 
* **2024-10-13**
 * improve [Toro C Library](https://github.com/KilianKegel/toro-C-Library/blob/master/README.md#20241013-v087-build-200)<br>
    * fixed: removed  disassembled math function wasn't replaced by extracted intrinsic 
    math function from Microsoft **LIBCMT.LIB**:
        * `ftol3.obj`
        * `ullshr.obj`
        * `ullrem.obj`
        * `ulldvrm.obj`
        * `ulldiv.obj`
        * `llshr.obj`
        * `llshl.obj`
        * `llrem.obj`
        * `llmul.obj`
        * `lldvrm.obj`
        * `lldiv.obj`
        original Microsoft functions are now available in the **toro C Library** for 32Bit.
    * **NEW**: Introduce **preliminary alpha** version of `MATH.H` functions<br>
        **NOTE**: Use functions below fails with special parameters.<br>
        **It is recommenDed not to use these functions in productive code.**<br>
        * [`acos()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/acos.c)
        * [`asin()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/asin.c)
        * [`atan()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/atan.)
        * [`atan2()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/atan2.c)
        * [`ceil()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/ceil.c)
        * [`cos()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/cos.c)
        * [`cosh()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/cosh.c)
        * [`exp()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/exp.c)
        * [`fabs()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/fabs.c)
        * [`floor()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/floor.c)
        * [`fmod()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/fmod.c)
        * [`frexp()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/frexp.c)
        * [`ldexp()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/ldexp.c)
        * [`log()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/log.c)
        * [`log10()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/log10.c)
        * [`modf()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/modf.c)
        * [`pow()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/pow.c)
        * [`sin()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/sinc.)
        * [`sinh()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/sinh.c)
        * [`sqrt()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/sqrt.c)
        * [`tan()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/tan.c)    
        * [`tanh()`](https://github.com/KilianKegel/Visual-TORO-C-LIBRARY-for-UEFI/blob/main/toroCLibrary/Library/math_h/tanh.c)
* **2024-09-08**
 * improve [Toro C Library](https://github.com/KilianKegel/toro-C-Library/blob/master/README.md#20240908-v086-build-187)<br>
   `system()` call on **UEFI Shell** now also working with output redirection.
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

