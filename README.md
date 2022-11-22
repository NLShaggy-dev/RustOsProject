# RustOsProject

following [blog_os](https://os.phil-opp.com/) project for build a rust os

### to build

```
cargo build
```

### to build bootimage

1. install bootimage tool
```
cargo install bootimage
```

2. add the `llvm-tools-preview` component
```
rustup component add llvm-tools-preview
```

3. run the bootimage script
```
cargo bootimage
```

image is found in `{project dir}/target/x86_64-blog_os/debug/bootimage-blog_os.bin`


### testing changes in image
to boot up and test our image locally we can use qemu so install that.

to run the runner in the project from bootimage script just do `cargo run`

### integration tests
```
cargo test
```