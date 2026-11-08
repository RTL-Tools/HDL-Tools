# HDL Tools

One-click install for the HDL-* VS Code extensions. Installing this pack installs:

| Extension | What it does |
|---|---|
| [HDL-AutoDoc-Lite](https://github.com/RTL-Tools/HDL-AutoDoc) | Generates documentation from your HDL source. |
| [HDL Log Lens](https://github.com/RTL-Tools/HDL-Log-Lens) | Turns HDL tool logs (NVC, Verilator, Yosys, nextpnr) into clickable VS Code problems. |
| [HDL Outliner](https://github.com/RTL-Tools/HDL-Outliner) | Sidebar outline of SV/Verilog/VHDL files: instances, types, constants, signals. |

The extensions stay independent. Uninstalling the pack leaves them installed, and each updates on its own.

## Releasing

Push a tag `vX.Y.Z` that matches `package.json`'s version. The Publish workflow packages the pack and publishes it to the Marketplace (trusted publishing, no token) and attaches the `.vsix` to a GitHub release.

To add an extension to the pack, add its ID to `extensionPack` in `package.json` and the table above.
