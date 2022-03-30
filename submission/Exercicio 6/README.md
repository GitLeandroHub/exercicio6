# pallet-kitties
Exercicio 6:
- Run benchmark related commands and see if the output makes sense
    - `make benchmark`
    - `cargo test --manifest-path pallets/kitties/Cargo.toml --features runtime-benchmarks -- --nocapture`
      ![](make-bench.png)

    - `make benchmark-output`
		- `cargo run --manifest-path node/Cargo.toml --release --features runtime-benchmarks -- benchmark --extrinsic '*' --pallet pallet_kitties --output pallets/kitties/src/weights.rs --template=frame-weight-template.hbs --execution=wasm --wasm-execution=compiled`
    ![](bench-outpupt.png)

    - `make benchmark-traits`
		- `cargo run --manifest-path node/Cargo.toml --release --features runtime-benchmarks -- benchmark --extrinsic '*' --pallet pallet_kitties --output runtime/src/weights/pallet_kitties.rs --execution=wasm --wasm-execution=compiled`
    ![](bench-traits.png)
    
    - `cargo run --manifest-path node/Cargo.toml --features runtime-benchmarks -- benchmark --help`
    ![](bench-help.png)

    - `cargo run --manifest-path node/Cargo.toml --features runtime-benchmarks -- benchmark --extrinsic '*' --pallet '*' --wasm-execution=compiled`
    ![](extrinsic-bench.png)
