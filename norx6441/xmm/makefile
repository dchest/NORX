CFLAGS=-O3 -march=native -std=c89 -Wall -pedantic -Wno-long-long

all: check bench

bench:
	@$(CC) $(CFLAGS) -o bench ../../bench/bench.c norx64.c
	@./bench
	@rm bench

check:
	@$(CC) $(CFLAGS) -I. -o check ../../check/check.c norx64.c
	@./check
	@rm check
