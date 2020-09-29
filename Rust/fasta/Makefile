compile:
	cargo build

measure:
	sudo modprobe msr
	sudo ../../RAPL/main "cargo run 25000000" Rust fasta

run:
	cargo run 25000000

mem:
	/usr/bin/time -v cargo run 25000000

valgrind:
	valgrind --tool=massif --stacks=yes cargo run 25000000
