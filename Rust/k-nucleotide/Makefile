compile:
	cargo build

measure:
	sudo modprobe msr
	sudo ../../RAPL/main "cargo run < knucleotide-input25000000.txt" Rust k-nucleotide

run:
	cargo run < knucleotide-input25000000.txt

mem:
	/usr/bin/time -v cargo run < knucleotide-input25000000.txt

valgrind:
	valgrind --tool=massif --stacks=yes cargo run < knucleotide-input25000000.txt
