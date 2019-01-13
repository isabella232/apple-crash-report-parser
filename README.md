# Apple Crash Report Parser

[![Build Status](https://travis-ci.com/getsentry/apple-crash-report-parser.svg?branch=master)](https://travis-ci.org/getsentry/apple-crash-report-parser)
[![Crates.io](https://img.shields.io/crates/v/apple-crash-report-parser.svg?style=flat)](https://crates.io/crates/apple-crash-report-parser)

This is a Rust library that can parse apple crash report text files.  These files
are generated by the apple native crash reporter as well as PLCrashReporter and
KSCrash.

## Example file

```
Incident Identifier: 5C32DF84-31A0-43E7-87D0-239F7F594940
CrashReporter Key:   TODO
Hardware Model:      MacBookPro14,3
Process:         YetAnotherMac [49028]
Identifier:      com.YourCompany.YetAnotherMac
Version:         4.21.1
Code Type:       X86-64
Parent Process:  launchd [1]

Date/Time:       2019-01-09 17:44:22 +0000
OS Version:      Mac OS X 10.14.0 (18A391)
Report Version:  104

Exception Type:  SIGSEGV
Exception Codes: SEGV_MAPERR at 0x88
Crashed Thread:  5

Thread 0:
0   libsystem_kernel.dylib              0x00007fff61bc6c2a 0x7fff61bc6000 + 3114
1   CoreFoundation                      0x00007fff349f505e 0x7fff349b9000 + 245854
2   CoreFoundation                      0x00007fff349f45ad 0x7fff349b9000 + 243117
3   CoreFoundation                      0x00007fff349f3ce4 0x7fff349b9000 + 240868
4   HIToolbox                           0x00007fff33c8d895 0x7fff33c83000 + 43157
5   HIToolbox                           0x00007fff33c8d5cb 0x7fff33c83000 + 42443
6   HIToolbox                           0x00007fff33c8d348 0x7fff33c83000 + 41800
7   AppKit                              0x00007fff31f4a95b 0x7fff31f30000 + 108891
8   AppKit                              0x00007fff31f496fa 0x7fff31f30000 + 104186
9   AppKit                              0x00007fff31f4375d 0x7fff31f30000 + 79709
10  YetAnotherMac                       0x0000000108b7092b 0x10864e000 + 5384491
11  YetAnotherMac                       0x0000000108b702a6 0x10864e000 + 5382822
12  libdyld.dylib                       0x00007fff61a8e085 0x7fff61a77000 + 94341

...
```

## Resources

- [crates.io](https://crates.io/crates/apple-crash-report-parser)
- [Documentation](https://docs.rs/apple-crash-report-parser)
