# How to reproduce

- Clone this repo on a Windows machine;
- go into the `bar` folder;
- run `cargo test --doc`;
- you should see a `Test executable failed (exit code: 0xc0000135).` error.

# Workarounds

- Add `%RUSTUP_HOME%\toolchains\stable-x86_64-pc-windows-msvc\lib\rustlib\x86_64-pc-windows-msvc\lib\` to the `PATH` environment variable;
- or alternatively copy the `std-somehashhere.dll` file to the `bar/` directory.

# Upstream issues

- https://github.com/rust-lang/rust/issues/39487
- https://github.com/rust-lang/rustup/issues/893
