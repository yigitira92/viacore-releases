# Third-Party Notices

ViaCore Proxy Management includes the following third-party component. This file is provided to
satisfy redistribution notice requirements; it is not legal advice.

---

## WinDivert 2.2.2

- **Homepage:** https://www.reqrypt.org/windivert.html
- **Source / releases:** https://github.com/basil00/WinDivert
- **Version used:** 2.2.2 (package `WinDivert-2.2.2-A.zip`, SHA-256 `63cb41763bb4b20f600b6de04e991a9c2be73279e317d4d82f237b150c5f3f15`)
- **License:** GNU Lesser General Public License v3 (LGPLv3) **OR** GNU General Public License v2 (GPLv2), at your option.
- **Use in ViaCore:** ViaCore links to WinDivert's user-mode API DLL (`WinDivert.dll`) at run time and
  relies on WinDivert's signed kernel driver (`WinDivert64.sys`) for local network interception.
  The WinDivert binaries are redistributed **unmodified**. ViaCore does not build WinDivert from source
  and does not incorporate WinDivert source code into ViaCore's own (proprietary) source.

ViaCore uses WinDivert under the terms of the **LGPLv3**. Under the LGPLv3, the covered library
(WinDivert) may be used by a larger work provided the library itself remains replaceable and its
license and notices are conveyed. The complete WinDivert license text is distributed with ViaCore at
`third_party/WinDivert/LICENSE` and is installed alongside the product. The corresponding WinDivert
source code is available from the project homepage and release page listed above.

The WinDivert kernel driver (`WinDivert64.sys`) is Authenticode-signed by its signing sponsor
(Chengdu Mistiny Technology Co., Ltd). ViaCore neither re-signs nor alters this binary.

> WinDivert availability, its signature lifecycle, and future Windows kernel-driver trust policies are
> external to ViaCore and outside ViaCore's control.
