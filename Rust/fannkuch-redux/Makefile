compile:
	cargo build

measure:
	sudo modprobe msr
	sudo cgexec -g perf_event:bench ../../RAPL/main "cargo run 12" Rust fannkuch-redux

run:
	cargo run 12

mem:
	/usr/bin/time -v cargo run 12

valgrind:
	valgrind --tool=massif --stacks=yes cargo run 12
