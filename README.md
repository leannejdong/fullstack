# Fullstack Webapp on the cloud

## Locally

* `cargo run` in backend

[Note, your Rust toolchain using the root account. This can be fixed by changing the user and group permissions of .rustup.

`sudo chown -R xyz:xyz /home/xyz/.rustup`
rustup update
If your `/home/xyz/.cargo` is also owned by root you will probably want to fix that too.

* `trunk serve` in frontend

## With docker

Run `docker build -t taskapp .` in the parent directory.