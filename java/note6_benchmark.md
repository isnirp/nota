# Microbenching
- Micro-benchmarking is the process of measuring the performance of a small piece of code
- When benchmarking a unit of work from the JVM environment, the System.currentTimeMillis() or System.nanoTime() methods are typically used.
- JMH may be used to perform micro benchmarking on code units, while Jmeter can be used to perform performance testing on applications.

## why benchmarking tool like jmh, Caliper, Japex, or JUnitPerf
- However, taking measurements in this method has significant drawbacks. Some of these problems are caused by the JVM, while others are caused by the operating system. The most common issues are ignoring the trash collector’s influence, JVM optimizations, and JIT compilers