CFLAGS=-O3 -march=armv7-a -mcpu=cortex-a9 -mfpu=neon -std=c99 -Wall -pedantic -Wno-long-long

all: check bench

bench:
	@$(CC) $(CFLAGS) -o bench ../../bench/bench.c norx32.c
	@./bench
	@rm bench

check:
	@$(CC) $(CFLAGS) -I. -o check ../../check/check.c norx32.c
	@./check
	@rm check

