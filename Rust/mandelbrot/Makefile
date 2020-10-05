compile:
	cargo build

measure:
	sudo modprobe msr
	sudo cgexec -g perf_event:bench ../../RAPL/main "cargo run 16000" Rust mandelbrot

run:
	cargo run 16000

mem:
	/usr/bin/time -v  cargo run 16000

valgrind:
	valgrind --tool=massif --stacks=yes  cargo run 16000
