---
tags:
  - sed
---

# Intro
awk and sed are working together
- awk is more for processing columns
- sed is more for processing lines

## Example1

```bash
eric@MacBookPro LinuxNotes % ll
total 24
-rw-r--r--@ 1 eric  staff   59 Jan  9 19:06 awk.md
-rw-r--r--@ 1 eric  staff  126 Jan  9 19:07 sed.md
-rw-r--r--@ 1 eric  staff    5 Jan  9 19:02 test.md
eric@MacBookPro LinuxNotes % ll | sed 's/awk/asdf/'
total 24
-rw-r--r--@ 1 eric  staff   59 Jan  9 19:06 asdf.md
-rw-r--r--@ 1 eric  staff  126 Jan  9 19:07 sed.md
-rw-r--r--@ 1 eric  staff    5 Jan  9 19:02 test.md
eric@MacBookPro LinuxNotes %
```

## Example 2
Another example

```bash
eric@MacBookPro LinuxNotes % ll | awk '{print $5}'

59
622
5
eric@MacBookPro LinuxNotes %
```

