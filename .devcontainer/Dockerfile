FROM mcr.microsoft.com/devcontainers/rust:latest
 
RUN apt update && apt upgrade -y
RUN apt install coz-profiler

USER vscode
RUN rustup component add rustfmt clippy
RUN rustup target add x86_64-pc-windows-msvc
RUN cargo install cargo-watch cargo-nextest cargo-xwin
