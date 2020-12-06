# Bit_Serial
Simulations and designs for bit serial TTL circuitry and cpu architectures - using H. Neeman's "Digital"


Bit serial refers to a technique used in the design of CPU and DSP architectures - such that data is processed in a serial fashion - usually 1 bit at a time (though 2-bit and 4-bit methods are also used sometimes).

History

Up until 1951, all commercial and experimental CPUs used a bit serial architecture. This is partly because most of the viable memory sub-systems at that time created data that was input and output in a serial fashion. Secondly it minimised the amount of hardware required for the switching and routing of signals, and this allowed machines to be build within the hardware constraints of the day - i.e. vacuum tube technology.

As a bit serial machine processes its data sequentially, one bit at a time, the time to perform a calculation is directly related to the number of bits contained in the word. EDSAC (1949) used either a short 35 bit word or a long 71 bit word. This allowed mathematical precision to be maintained during calculations, but by modern standards EDSAC was a slow machine capable of about 600 operations per second.

With the advent of minicomputers, several manufacturers offered serial designs including the LGP-30 (1956), the LGP-400 (1960) and the LGP-21 (1963). These machines were relatively low cost and found their way into industry and education. Other notable bit serial machines are the Elliott Bros. 803 and the DEC PDP-8S. Whilst computationally slow - these machines were some of the first affordable minicomputers.

With the arrival of fast semiconductor memory and small scale integration of integrated circuits, bit serial fell out of fashion at the end of the 1960's for minicomputers, but instead the technology was adapted for the first of the electronic "Desktop" calculators. Bit serial arithmetic provided the means to create a basic "4 function" calculator using about a dozen ICs. Some of the first MSI ICs produced in Japan, from 1968 onwards, were serial adder-subtractor chips, and shift-registers of 48 or 60 bits to hold 12 or 15 BCD digits in serial form.

Bit serial found new life in the 70's and 80's as computationally intensive operations - such as CORDIC, and DSP operations such as FFT could be performed efficiently in bit serial hardware architectures, often based around small but flexible gate arrays and other programmable logic devices. 

Why Bit Serial in 2020?

Bit serial designs directly trade off their hardware complexity against their processing speed. If you want a simple soft-core processor on an FPGA, and and have few performance constraints, then a bit serial design might be an ideal use of the remaining hardware resources. With a bit serial design requiring minimal hardware, there exists the opportunity to have multiple bit serial cpu cores on a single FPGA.  
