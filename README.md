linpackc
========

The Linpack benchmark code measures floating point computation
performance. It was developed as part of the Linpack matrix
library. For more information, see the [Linpack Benchmark FAQ].

This code has been modified only to compile and run on the [Raspberry
Pi] and Mac OS X.

## Compiling and Running

Compile the code with the command:

    gcc -O4 -DDP -DROLL -o linpackc linpack.c -lm

This compiles the benchmark using double precision (-DDP) values and
not unrolling the loops (-DROLL). Use -DSP for single precision values
and -DUNROLL to unroll the loops.

Run the benchmark with the command:

    ./linpackc



[Linpack Benchmark FAQ]: http://www.netlib.org/utk/people/JackDongarra/faq-linpack.html

[Raspberry Pi]: http://www.raspberrypi.org/