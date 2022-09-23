Template for rust programming

## Usage

Install [cargo-generate](https://github.com/cargo-generate/cargo-generate) and cargo-run-script. Unless you did that before, run this line now:
```shell
cargo install cargo-generate --features vendored-openssl
cargo install cargo-run-script
```
Now, use it to create your new contract. Go to the folder in which you want to place it and run:
```shell
cargo generate --git https://github.com/phamnam1805/rust-template --name PROJECT_NAME
```

Then, go to Cargo.toml, change `profile.release.package.rust-template` to `profile.release.package.PROJECT_NAME`

## Create rust file 
```Shell
cd src
cargo new <src name>
```
Example 
```Shell
cd src
cargo new src-template
```
## Compile
Run `optimizer.sh` to compile code

## Run 
- In root directory of project:
```Shell
cargo run --bin <src name>
```
Example
```Shell
cargo run --bin src-template
```

- In each directory of `src`:
Example in src/src-template/
```Shell
cargo run
```