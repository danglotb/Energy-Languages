compile:
	cp -L binarytrees.node binarytrees.js
measure:
	sudo modprobe msr
	sudo cgexec -g perf_event:bench ../../RAPL/main "node binarytrees.js 21" JavaScript binary-trees

run:
	node binarytrees.js 21

mem:
	/usr/bin/time -v node binarytrees.js 21

valgrind:
	valgrind --tool=massif --stacks=yes node binarytrees.js 21
