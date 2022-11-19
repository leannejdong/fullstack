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

If your app uses AWS, you might pass the AWS credential

`docker run -p80:80 -t -e 'AWS_ACCESS_KEY_ID=$AWS_ACCESS_KEY_ID' -e 'AWS_SECRET_ACCESS_KEY=$AWS_SECRET_ACCESS_KEY' -e 'AWS_REGION=us-east-2' taskapp`