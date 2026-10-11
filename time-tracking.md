# E6 Systems - The 12,000-hour Journey
Time-tracking journal for e6, documenting a 12,000-hour journey. This journey is milestoned at 12-hour intervals.

## 2026-10-12 84-hour Milestone
Got the first working version of `e6_uefi_print_uefi_string`. The function prints a UEFI string pointed to in RSI. UEFI strings are UTF16 and null-terminated.
- Add idea for getting started coding to the ebook.
- Add reason for the decision to write e6_uefi_print_uefi_string first to the book fragments.
- First working version of e6_uefi_print_uefi_string.
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
