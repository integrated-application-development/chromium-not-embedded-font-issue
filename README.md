# chromium-not-embedded-font-issue

This repository contains two PDFs:

- [verdana-embedded.pdf](verdana-embedded.pdf)
- [verdana-not-embedded.pdf](verdana-not-embedded.pdf)

Our expectation is that these two PDFs should match in appearance; regular fonts appear regular,
bolded fonts appear bolded, italic fonts appear italicised. Something like below:

![image](expected.png)

However, in some newer versions of Chromium, the `verdana-not-embedded.pdf` file does not render
the bold font correctly. Typically, you'll see something like below instead in those browsers:

![image](actual.png)

We've tested these vendors, versions, and platforms:
| Vendor | Version | Platform | Embedded | Not Embedded |
| - | - | - | - | - |
| Chrome | 128 | Windows 10 | ✔ | ✔ |
| Chrome | 129 | Mac OS X 15 | ✔ | ✔ |
| Chrome | 129 | Windows 10 | ✔ | ❌ |
| Chrome | 131 | Ubuntu 22 | ✔ | ❌ |
| Chrome | 133 | Windows 10 | ✔ | ❌ |
| Chrome | Safari/604 | iOS 18 | ✔ | ✔ |
| Google Drive | 2.24 | Android 15 | ✔ | ❌ |
| Edge | 130 | Windows 10 | ✔ | ✔ |
| Edge | 131 | Mac OS X 15 | ✔ | ✔ |
| Edge | 131 | Windows 10 | ✔ | ❌ |
| Edge | 131 | Android 15 | ✔ | ❌ |
| Edge | 131 | Ubuntu 22 | ✔ | ❌ |
| Edge | 132 | Windows 10 | ✔ | ❌ |
| Firefox | 132 | Windows 10 | ✔ | ✔ |
| Firefox | 132 | Android 15 | ✔ | ✔ |
| Firefox | 133 | Ubuntu 22 | ✔ | ✔ |
| Safari | 18 | Mac OS X 15 | ✔ | ✔ |
| Safari | 605 | iOS 18 | ✔ | ✔ |
| Foxit | 2024.3 | Windows 10 | ✔ | ✔ |
| Adobe Acrobat | 24 | Windows 10 | ✔ | ✔ |
