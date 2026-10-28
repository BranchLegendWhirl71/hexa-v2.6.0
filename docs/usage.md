# Usage

## Requirements

- C++20
- Windows 10 or 11 (or the platform listed in the README)

## Install

1. Download and unpack Hexa.
2. Run hexa.exe as administrator.
3. Attach to a process you own or are authorized to test.
4. Run a first scan, then narrow it with next scans.
5. Save hits to a table and freeze the ones you need.

## Configuration

```text
%APPDATA%\Hexa\
├── config.ini
├── profiles\
└── logs\
```

- Run as administrator for full access.
- Only target processes you own or are authorized to test.
- Tables are portable JSON.

## Commands

```text
# attach and scan
hexa.exe --attach notepad.exe

# lua
local a = attach('notepad.exe')
local hits = scan(a, 'int', 100)
write(a, hits[1].address, 250)
freeze(a, hits[1].address, 250)
```

## Uninstall

Delete the application folder and `%APPDATA%\Hexa`. No services, no
drivers, no scheduled tasks are installed.