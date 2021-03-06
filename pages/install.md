extends: default.liquid
title: Install
path: install/
---

If you've already installed RLS via rustup, then you can skip this step and go
straight to setting up your [editor](/).

## Install rustup

You can install [rustup](http://rustup.rs/) on many platforms. This will help
us quickly install the RLS and its dependencies.

If you already have rustup installed, be sure to run self update to ensure you
have the latest rustup:

```
rustup self update
```

## Install nightly

Install the nightly compiler. You don't have to use it as your default
compiler, but it needs to be on your system:

```
rustup install nightly
```

## Install the RLS

Once you have rustup installed, run the following commands:

```
rustup component add rls --toolchain nightly
rustup component add rust-analysis --toolchain nightly
rustup component add rust-src --toolchain nightly
```

If you've never set up Racer before, you'll need to set up your RUST_SRC_PATH
variable. To do so, you can follow the [Racer configuration
steps](https://github.com/phildawes/racer#configuration)
