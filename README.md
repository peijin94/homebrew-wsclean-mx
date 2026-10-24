# wsclean-mx Homebrew tap

Native Apple Silicon CPU builds of [wsclean-mx](https://github.com/peijin94/wsclean-mx).

```sh
brew tap peijin94/wsclean-mx
brew tap ska-sa/tap
brew install ska-sa/tap/casacore-data
brew install peijin94/wsclean-mx/wsclean-mx
wsclean-mx -version
```

Upgrade an existing installation:

```sh
brew update
brew upgrade peijin94/wsclean-mx/wsclean-mx
```

Starting with **0.1.1**, the executable is **`wsclean-mx`**, not `wsclean`.
Update scripts accordingly; this package does not install an alias that shadows
upstream WSClean. The MX release version is printed separately from the pinned
upstream WSClean 3.7 version.

The formula builds CPU-only, including `--HEAD`. Experimental Metal is not
compiled into release bottles. Homebrew pours a compatible bottle when one is
available for the host platform, otherwise it builds from the pinned source.
The formula requires Apple Silicon and macOS Sequoia or newer; that does not
imply every supported OS has a prebuilt bottle or was tested by this release.

Release scope, evidence and remaining numerical-validation limitations are in
the project's [0.1.1 release notes](https://github.com/peijin94/wsclean-mx/releases/tag/v0.1.1)
and [installation guide](https://github.com/peijin94/wsclean-mx/blob/release/0.1.1/install.md).
