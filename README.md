# myron-ios kernel build

Minimal build tree used to produce the xnu kernel for the Redmi K90 Pro Max
(SM8850, myron/songyuan). Built on GitHub Actions macOS.

Contents:
- `xnu/patches/` — the xnu-8796 patch series (from ios-sweet / ios-fuxi, plus the
  SM8850 board patches). See those projects for licenses and history.
- `songyuan/adapt.py` — rewrites the board constants in the patches for this panel.
- `.github/workflows/xnu-songyuan-v5.yml` — the build workflow (macOS 14, Xcode 15).

This repository exists only to run the build. It is removed once the kernel
artifact has been downloaded.
