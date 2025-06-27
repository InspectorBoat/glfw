# GLFW packaged for the Zig build system

This is a fork of [glfw](https://github.com/glfw/glfw), packaged for Zig. Unnecessary files have been deleted, and the build system has been replaced with build.zig.

This was once maintained by Mach Engine, but was abandoned and moved to a personal repository, which was then deleted. This is a reupload, pulled from [https://pkg.machengine.org/glfw/ec656e10d3643a3a71149bb96ae6b0831b84b677.tar.gz](https://pkg.machengine.org/glfw/ec656e10d3643a3a71149bb96ae6b0831b84b677.tar.gz) and "rebased" on glfw at the time of upload, as the package pulled from pkg.machengine.org did not include git history. (The rebase was done manually, by cloning https://github.com/glfw/glfw and manually making changes to match the archived package.)

_Looking for Zig bindings to GLFW?_ See [inspectorboat/mach_glfw](https://github.com/inspectorboat/mach_glfw).

## Updating

To update this repository, run `./update.sh` followed by `./verify.sh` to verify the repository contents.

## Verifying repository contents

For supply chain security reasons (e.g. to confirm we made no patches to the code) we provide a `git diff` command you can run to verify the contents of this repository:

```sh
./verify.sh
```

If nothing is printed, there is no diff. Deleted files, and changes to `README.md`, `build.zig`, `.github` CI files and `.gitignore` are ignored.