`crashpad` library - Build2 package
================================

 - crashpad : https://chromium.googlesource.com/crashpad/crashpad
 - Build2 : https://build2.org

Note: This is the source code for the build2 package of the `crashpad` C++ library,
the actual library sources snapshot can be found in the `./upstream/` submodule.

Supported:
 - linux (gcc/clang)
 - windows-static (msvc)
 - macos-static (clang)

TODO:
 - Get `linux_syscall_support.h` via a git submodule.
 - Rename `lib{getopt}` to `lib{crashpad_getopt}`.
 - Add `cxx.pkgconfig.include` for all libraries (see `lib{crashpad_build}` for an example).
 - `zlib_crashpad.h` is included by public headers and therefore must be
   installed. Perhaps it's cleaner to just make it into a (header-only)
   library like getopt (e.g., `lib{crashpad_zlib}`).

 - Add support for (Android/ChromeOS/IOS/Fuchsia)
 - Investigate disabled tests
