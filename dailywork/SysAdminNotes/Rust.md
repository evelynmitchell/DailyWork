
```
$ rustup
rustup 1.26.0 (2024-04-01)
The Rust toolchain installer

USAGE:
    rustup [OPTIONS] [+toolchain] <SUBCOMMAND>

ARGS:
    <+toolchain>    release channel (e.g. +stable) or custom
                    toolchain to set override

OPTIONS:
    -v, --verbose    Enable verbose output
    -q, --quiet      Disable progress output
    -h, --help       Print help information
    -V, --version    Print version information

SUBCOMMANDS:
    show           Show the active and installed toolchains or
                       profiles
    update         Update Rust toolchains and rustup
    check          Check for updates to Rust toolchains and
                       rustup
    default        Set the default toolchain
    toolchain      Modify or query the installed toolchains
    target         Modify a toolchain's supported targets
    component      Modify a toolchain's installed components
    override       Modify directory toolchain overrides
    run            Run a command with an environment
                       configured for a given toolchain
    which          Display which binary will be run for a
                       given command
    doc            Open the documentation for the current
                       toolchain
    man            View the man page for a given command
    self           Modify the rustup installation
    set            Alter rustup settings
    completions    Generate tab-completion scripts for your
                       shell
    help           Print this message or the help of the given
                       subcommand(s)

DISCUSSION:
    Rustup installs The Rust Programming Language from the
official
    release channels, enabling you to easily switch between
stable,
    beta, and nightly compilers and keep them updated. It makes
    cross-compiling simpler with binary builds of the standard
library
    for common platforms.

    If you are new to Rust consider running `rustup doc --book` to
    learn Rust.
```
## book

```
rustup doc --book
info: syncing channel updates for 'stable-x86_64-unknown-linux-gnu'
info: latest update on 2025-03-18, rust version 1.85.1 (4eb161250 2025-03-15)
info: downloading component 'cargo'
info: downloading component 'clippy'
info: downloading component 'rust-docs'
info: downloading component 'rust-std'
info: downloading component 'rustc'
info: downloading component 'rustfmt'
info: installing component 'cargo'
info: installing component 'clippy'
info: installing component 'rust-docs'
 18.2 MiB /  18.2 MiB (100 %)   6.4 MiB/s in  2s ETA:  0s
info: installing component 'rust-std'
 29.2 MiB /  29.2 MiB (100 %)  10.8 MiB/s in  2s ETA:  0s
info: installing component 'rustc'
 69.5 MiB /  69.5 MiB (100 %)  11.7 MiB/s in  5s ETA:  0s
info: installing component 'rustfmt'
```

https://rust-book.cs.brown.edu/

file:///home/efm/.rustup/toolchains/stable-x86_64-unknown-linux-gnu/share/doc/rust/html/book/index.html

## version
```bash
$ rustc --version
rustc 1.85.1 (4eb161250 2025-03-15)
```

## update
```bash  
$ rustup update
info: syncing channel updates for 'stable-x86_64-unknown-linux-gnu'
info: cleaning up downloads & tmp directories
```

## uninstall 
```bash
$ rustup self uninstall
```

## compile
```bash
$ rustc main.rs
```

## set version
```bash
$ rustc main.rs
error: rustup could not choose a version of rustc to run, because one wasn't specified explicitly, and no default is configured.
help: run 'rustup default stable' to download the latest stable release of Rust and set it as your default toolchain.
$ rustup default stable
info: using existing install for 'stable-x86_64-unknown-linux-gnu'
info: default toolchain set to 'stable-x86_64-unknown-linux-gnu'

  stable-x86_64-unknown-linux-gnu unchanged - rustc 1.85.1 (4eb161250 2025-03-15)
```

## run
```bash
$ rustc main.rs
$ ./main
Hello, world!
```

## format
```bash
$ rustfmt
```

## package manager
```bash
$ cargo --version
cargo 1.85.1 (d73d2caf9 2024-12-31)
```

## new project
git repo is automatically created
```bash
$ cargo new hello_cargo
    Creating binary (application) `hello_cargo` package
note: see more `Cargo.toml` keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
$ cd hello_cargo
$ ls
Cargo.toml  src
$ cd src
$ ls
main.rs
```
## cargo.toml
```toml
[package]
name = "hello_cargo"
version = "0.1.0"
edition = "2024"

[dependencies]
```

## build and run cargo project
### build
From within hello_cargo
```bash
$ ~/git/myrepos/rusttuorial/hello_cargo$ cargo build
   Compiling hello_cargo v0.1.0 (/home/efm/git/myrepos/rusttuorial/hello_cargo)
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.22s
```
This command creates an executable file in _target/debug/hello_cargo
```bash
~/git/myrepos/rusttuorial/hello_cargo$ ls
Cargo.lock  Cargo.toml  src  target
~/git/myrepos/rusttuorial/hello_cargo$ ls target
CACHEDIR.TAG  debug
~/git/myrepos/rusttuorial/hello_cargo$ ls target/debug
build  deps  examples  hello_cargo  hello_cargo.d  incremental
```

###  run
```bash
$ ~/git/myrepos/rusttuorial/hello_cargo$ ./target/debug/hello_cargo
Hello, world!
```
or
```bash
~/git/myrepos/rusttuorial/hello_cargo$ cargo run
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.01s
     Running `target/debug/hello_cargo`
Hello, world!
```

## check
```bash
~/git/myrepos/rusttuorial/hello_cargo$ cargo check
    Checking hello_cargo v0.1.0 (/home/efm/git/myrepos/rusttuorial/hello_cargo)
    Finished `dev` profile [unoptimized + debuginfo] target(s) in 0.05s
```

## build for release
```bash
~/git/myrepos/rusttuorial/hello_cargo$ cargo build --release
   Compiling hello_cargo v0.1.0 (/home/efm/git/myrepos/rusttuorial/hello_cargo)
    Finished `release` profile [optimized] target(s) in 0.17s
```
### run release
```bash
~/git/myrepos/rusttuorial/hello_cargo$ cargo run --release
    Finished `release` profile [optimized] target(s) in 0.01s
     Running `target/release/hello_cargo`
Hello, world!
```

## test
```bash
$ cargo test
```