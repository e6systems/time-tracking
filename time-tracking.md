# E6 Systems - The 12,000-hour Journey
Time-tracking journal for e6, documenting a 12,000-hour journey. This journey is milestoned at 12-hour intervals.

## 2026-10-20 96-hour Milestone
Started this milestone with some brainstorming on e6os's installer. Rewrote some parts of the installer bootloader. Added a proper `.bss` section and adjusted some values in the PE32+ headers. This is done with `section .bss nobits`. `nobits` tells NASM that the section is just for address calculations and should not appear in the final compiled binary.
- Locating Handle Buffer seems to work now (LocateHandleBuffer).
- Add ideal location for `struc` in ebook fragment. 
- Add decision to use `struc` in the ebook fragment.
- Add caution to encourage using `struc` in ebook fragment.
- Got the installer working using `struc` and rewriting the BSS section. 
- Used `struc` to organize the .bss section.
- Still brainstorming on enumeration of storage devices.
- Added chapter idea to the ebook.
- Rewrote the installer bootloader for stricter firmware.
- Add `.bss` section to the installer bootloader.
- Brainstormed and generated ideas for the e6os installer.
- Added a TODO to the book on installing qemu and nasm on Windows, Linux, and Mac.
- Add Wikipedia and FAT specifications to list of resources in the ebook.
- Brainstorming on enumerating storage devices.

## 2026-10-15 84-hour Milestone
Got the first working version of `e6_uefi_print_uefi_string`. The function prints a UEFI string pointed to in RSI. UEFI strings are UTF16 and null-terminated. Also got first working version `e6_uefi_dump_memory`. It dumps 256 consecutive bytes of memory on-screen. The memory address to dump is passed in RSI and must be 256 bytes aligned.
- Refactored the `e6_uefi_dump_memory` function.
- Got first working version of `e6_uefi_dump_memory`.
- Cleanup `e6_uefi_print_rax`.
- Got first working version of `e6_uefi_print_rax`.
- Started work on `e6_efi_print_rax`.
- Added stack alignment to `e6_uefi_print_uefi_string` function.
- Cleanup the `e6_uefi_print_uefi_string` function.
- Add idea for getting started coding to the ebook.
- Add reason for the decision to write `e6_uefi_print_uefi_string` first to the book fragments.
- First working version of `e6_uefi_print_uefi_string`.
- Add more info in ABI about checking and calculating the checksum.
- Brainstorm ideas for the ABI.
- Edit and update the ABI file.

## 2026-10-10 72-hour Milestone
Add some information to the Calling Convention and the ABI.
- Add into ABI about what happens on program entry.
- Update calling convention with information about fixed-width strings.
- Add info about slice records in the Calling Convention file.
- Add info about 'range-terminated' strings in the Calling Convention.
- Updated ABI with information about e6-executable binary header.
- Updated the Call Convention to contain info about data types I came up with especially the strings.
- Add clarifying information about buffers in the Call Convention.
- Do some minor cleanups.

## 2026-10-09 60-hour Milestone
Baseline.  
Initial ideas, setup and previous work that had been done.
- Wrote installer build and test script in bash. The script automatically launches qemu.
- The E6 installer successfully boots in UEFI, got the PE64 header working in NASM.
- Installer works with qemu.
- Added some fragments to the e6 book.
- Wrote out the build and test installer shell script.
- Setup this time-tracking repository.
- Created the e6 GitHub Organizations with repository for e6 compiler, e6 operating system and the e6 book.
- Brainstorming on book content and structure.
- Successfully built usb image for installer to be used with qemu.
