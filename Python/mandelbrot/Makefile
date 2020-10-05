compile:
	cp mandelbrot.python3-7.python3 mandelbrot.python3-7.py
measure:
	sudo modprobe msr
	sudo cgexec -g perf_event:bench ../../RAPL/main "python3 -OO mandelbrot.python3-7.py 16000" Python mandelbrot

run:
	python3 -OO mandelbrot.python3-7.py 16000

mem:
	/usr/bin/time -v python3 -OO mandelbrot.python3-7.py 16000
