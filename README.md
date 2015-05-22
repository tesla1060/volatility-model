##Introduction

A joint collaboration between the Finance and Financial Service and Business Analytics Lab of Loyola University Chicago. The goal of this project is to compare the time taken to compute the price of a binomial option by using The Cox–Ross–Rubinstein (CRR) procedure, followed by backward induction calculated on a regular machine against one that uses Maxeler computing. In Computer Science, a similar way of approach is by the **triangular wavefront** programming.

##Features of Maxeler Computing

-   **Field-Programmable Gate Array (FPGA)**

    Maxeler typically packs the Field-Programmable Gate Array (FPGA), made by Xilinx, in circuit boards that work with Intel Xeon microprocessors, whose unique chip allows for single and multiple data streams. Unlike traditional Read-Only Memory (ROM), the circuitry of these FPGAs gives the programmers flexibility to reconfigure data after it has been programmed into the chip.  It also supplies special software, called compilers, to exploit the hardware â€“ which can be continuously reprogrammed for customization to fit new sets of jobs. 
	
	
-   **Multiscale Dataﬂow Computing**

	In addition to the FPGA, Maxeler’s Multiscale DataﬂowComputing, a combination of traditional synchronous data flow, vector and array processor, allows for the manipulation of loop level parallelism in a spatial, pipelined way. Large streams of data ﬂowing through a sea of arithmetic units can be connected to match the structure of the computer task. Small on-chip memories form a distributed register ﬁle with as many access ports as needed to support a smooth ﬂow of data through the chip.

	Multiscale Dataﬂow Computing employs dataﬂow on multiple levels of abstraction: the system level,the architecture level, the arithmetic level and the bit level. On the system level, multiple dataﬂowengines are connected to form a supercomputer. On the architecture level, memory access can be decoupled from arithmetic operations, while the arithmetic and bit levels provide opportunities to optimize the representation of the data and balance computation with communication.

|Figure 1: An example of Dataflow Computing in Maxeler|
|:-------------:|
| ![Programmingwith MaxCompiler](https://github.com/davidtanluc/ParallelProgramming/raw/master/wiki1/MaxelerSlide9%20.PNG) |
| As illustrated in Figure 1, CPU codes (C language) are the main front to navigate data streaming into Engine Codes (MyKernel in Figure 1), which are written in Java for its data design expressions. The communication and translation between CPU codes and Engine codes are performed continuously.|


##Our approach

The Cox–Ross–Rubinstein (CRR) procedure, part of the Binomal Options Pricing Model, was provided in Excel VBA format by the Finance Department. The Computer Science Department converted these codes in Java for readability which would serve as a central point of reference between the original Excel VBA and the translated C language, which Maxeler computing exclusively uses for its CPU codes. The Financial Service and Business Analytics Lab covered the Java and C code to Maxeler Code.

Initially we built a controlled environment based on static data provided by the Finance Department (VBA model). The static data comprises of spot prices, dividend yields and other constants of a standard call option. Using the CRR formula, these data were used to calculate Implied Volatility (IV).

##Our findings

TODO

##Conclusion

TODO
