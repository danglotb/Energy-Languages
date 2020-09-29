compile:
	cargo build

measure:
	sudo modprobe msr
	sudo ../../RAPL/main "cargo run 21" Rust binary-trees

run:
	cargo run 21

mem:
	/usr/bin/time -v cargo run 21

valgrind:
	valgrind --tool=massif --stacks=yes cargo run 21
