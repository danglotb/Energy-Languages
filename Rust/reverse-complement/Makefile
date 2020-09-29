compile:
	cargo build

measure:
	sudo modprobe msr
	sudo ../../RAPL/main "cargo run < ../../revcomp-input25000000.txt" Rust reverse-complement

run:
	cargo run < ../../revcomp-input25000000.txt

mem:
	/usr/bin/time -v cargo run < ../../revcomp-input25000000.txt

valgrind:
	valgrind --tool=massif --stacks=yes cargo run < ../../revcomp-input25000000.txt
