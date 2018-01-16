# Releasing
We use [JitPack](https://jitpack.io) for releasing.

1. Switch to the `master` branch 
1. Merge the latest changes from `develop` into `master`
1. Update `build.gradle` and `README.md` with the new version number
1. Push `master` to GitHub
1. Create a new [GitHub Release](https://github.com/blog/1547-release-your-software). This is what triggers JitPack to build and release the library.
1. Merge `master` back into `develop` (to get the version number update), and update `build.gradle` with a new snapshot version (e.g. `1.0.0-SNAPSHOT`). This keeps the version of in-development builds separate from released builds.