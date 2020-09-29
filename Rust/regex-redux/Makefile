compile:
	cargo build

measure:
	sudo modprobe msr
	sudo ../../RAPL/main "cargo run 0 < ../../regexredux-input5000000.txt" Rust regex-redux

run:
	cargo run 0 < ../../regexredux-input5000000.txt

mem:
	/usr/bin/time -v cargo run 0 < ../../regexredux-input5000000.txt

valgrind:
	valgrind --tool=massif --stacks=yes cargo run 0 < ../../regexredux-input5000000.txt
