Log

```shell
crane-reproduce-no-backtrace-deps> +++ command cargo --version
crane-reproduce-no-backtrace-deps> cargo 1.92.0 (344c4567c 2025-10-21)
crane-reproduce-no-backtrace-deps> +++ command cargo check --release --locked --all-targets
crane-reproduce-no-backtrace-deps>    Compiling crane-reproduce-no-backtrace v0.1.0 (/nix/var/nix/builds/nix-98643-2561287373/source)
crane-reproduce-no-backtrace-deps>     Checking log v0.4.29
crane-reproduce-no-backtrace-deps>     Finished `release` profile [optimized + debuginfo] target(s) in 1.57s
crane-reproduce-no-backtrace-deps> +++ command cargo build --release --locked
crane-reproduce-no-backtrace-deps>    Compiling log v0.4.29
crane-reproduce-no-backtrace-deps>    Compiling crane-reproduce-no-backtrace v0.1.0 (/nix/var/nix/builds/nix-98643-2561287373/source)
crane-reproduce-no-backtrace-deps>     Finished `release` profile [optimized + debuginfo] target(s) in 0.30s
crane-reproduce-no-backtrace-deps> fixing up neutered remapped "/nix/store/n2k7k5lx8q7wjjcc7mmjppj28k5mkky0-source" source path references
crane-reproduce-no-backtrace-deps> Running phase: checkPhase
crane-reproduce-no-backtrace-deps> +++ command cargo test --release --locked --no-run
crane-reproduce-no-backtrace-deps>    Compiling crane-reproduce-no-backtrace v0.1.0 (/nix/var/nix/builds/nix-98643-2561287373/source)
crane-reproduce-no-backtrace-deps>     Finished `release` profile [optimized + debuginfo] target(s) in 0.13s
crane-reproduce-no-backtrace-deps>   Executable unittests src/main.rs (target/release/deps/crane_reproduce_no_backtrace-98b1cb12601ee05e)
crane-reproduce-no-backtrace-deps> Running phase: installPhase
crane-reproduce-no-backtrace-deps> incremental zstd compression not currently supported on Darwin: https://github.com/rust-lang/rust/issues/115982
crane-reproduce-no-backtrace-deps> doing a full archive install of target to /nix/store/qc378rap3zh72yysbxgfzxhl470kwfrv-crane-reproduce-no-backtrace-deps-0.1.0/target.tar.zst
crane-reproduce-no-backtrace-deps> /*stdin*\            : 18.40%   (  3.67 MiB =>    692 KiB, /nix/store/qc378rap3zh72yysbxgfzxhl470kwfrv-crane-reproduce-no-backtrace-deps-0.1.0/target.tar.zst)
crane-reproduce-no-backtrace-deps> Running phase: fixupPhase
crane-reproduce-no-backtrace-deps> checking for references to /nix/var/nix/builds/nix-98643-2561287373/ in /nix/store/qc378rap3zh72yysbxgfzxhl470kwfrv-crane-reproduce-no-backtrace-deps-0.1.0...
crane-reproduce-no-backtrace-deps> patching script interpreter paths in /nix/store/qc378rap3zh72yysbxgfzxhl470kwfrv-crane-reproduce-no-backtrace-deps-0.1.0
crane-reproduce-no-backtrace> Running phase: unpackPhase
crane-reproduce-no-backtrace> unpacking source archive /nix/store/rc3l6rsy47wm06w24j9bw683n9fsirqh-source
crane-reproduce-no-backtrace> source root is source
crane-reproduce-no-backtrace> Running phase: patchPhase
crane-reproduce-no-backtrace> Executing configureCargoCommonVars
crane-reproduce-no-backtrace> decompressing cargo artifacts from /nix/store/qc378rap3zh72yysbxgfzxhl470kwfrv-crane-reproduce-no-backtrace-deps-0.1.0/target.tar.zst to target
crane-reproduce-no-backtrace> Running phase: updateAutotoolsGnuConfigScriptsPhase
crane-reproduce-no-backtrace> Running phase: configurePhase
crane-reproduce-no-backtrace> will append /nix/var/nix/builds/nix-98643-2561287374/source/.cargo-home/config.toml with contents of /nix/store/cixwck7czh1vv41fm5lv2nffdl7n6p48-vendor-cargo-deps/config.toml
crane-reproduce-no-backtrace> default configurePhase, nothing to do
crane-reproduce-no-backtrace> Running phase: buildPhase
crane-reproduce-no-backtrace> configuring CARGO_BUILD_RUSTFLAGS to remap paths from "/nix/var/nix/builds/nix-98643-2561287374/source" to "/nix/store/rc3l6rsy47wm06w24j9bw683n9fsirqh-source"
crane-reproduce-no-backtrace>  - neutering as "/nix/store/####CRANE-NEUTERED-REMAP-SRC####-source" for source path remapping
crane-reproduce-no-backtrace> setting CARGO_BUILD_RUSTFLAGS= --remap-path-prefix=/nix/var/nix/builds/nix-98643-2561287374/source=/nix/store/####CRANE-NEUTERED-REMAP-SRC####-source
crane-reproduce-no-backtrace> +++ command cargo --version
crane-reproduce-no-backtrace> cargo 1.92.0 (344c4567c 2025-10-21)
crane-reproduce-no-backtrace> +++ command cargo build --release --message-format json-render-diagnostics --locked
crane-reproduce-no-backtrace>    Compiling log v0.4.29
crane-reproduce-no-backtrace>    Compiling crane-reproduce-no-backtrace v0.1.0 (/nix/var/nix/builds/nix-98643-2561287374/source)
crane-reproduce-no-backtrace>     Finished `release` profile [optimized + debuginfo] target(s) in 0.23s
crane-reproduce-no-backtrace> fixing up neutered remapped "/nix/store/rc3l6rsy47wm06w24j9bw683n9fsirqh-source" source path references
crane-reproduce-no-backtrace> searching for bins/libs to install from cargo build log at cargoBuildLogYjSy.json
crane-reproduce-no-backtrace> installing /nix/var/nix/builds/nix-98643-2561287374/source/target/release/crane-reproduce-no-backtrace in postBuildInstallFromCargoBuildLogOutTempcZJ/bin
```
