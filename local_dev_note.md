# Build release version
cargo clean
cargo build --profile release -p openfang-cli

# Build release-fast version
cargo clean
cargo build --profile release-fast -p openfang-cli

Note:
cargo clean is necessary because of the way Rust compiler caches work. If you switch between debug and release builds, clean first to ensure a full rebuild.
