compile:
	cargo build

measure:
	sudo modprobe msr
	sudo ../../RAPL/main "cargo run 5500" Rust spectral-norm

run:
	cargo run 5500

mem:
	/usr/bin/time -v cargo run 5500

valgrind:
	valgrind --tool=massif --stacks=yes cargo run 5500
