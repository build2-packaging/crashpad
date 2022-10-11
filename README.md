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
 - Add `LICENSE` file to -handler, -tools, and -tests.
 - Add support for (Android/ChromeOS/IOS/Fuchsia)
 - Investigate disabled tests
