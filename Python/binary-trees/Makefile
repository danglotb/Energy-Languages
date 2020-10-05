compile:
	cp binarytrees.python3 binarytrees.py

measure:
	sudo modprobe msr
	sudo cgexec -g perf_event:bench ../../RAPL/main "python3 -OO binarytrees.py 21" Python binary-trees

run:
	python3 -OO binarytrees.py 21

mem:
	/usr/bin/time -v python3 -OO binarytrees.py 21
