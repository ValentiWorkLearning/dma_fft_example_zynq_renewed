## A kind of a README

So. I was fighting with the FFT IP with DMA and baremetal applications. Finally the reference design provided by Xilinx seems to be more or less working as I expect!


For having this sample working with floats as well as with integers-fixed point the following changes were made to the block settings:
1. Adjustmenets for Stream Data Width, width of the buffer length register
![image](https://github.com/user-attachments/assets/81416302-1889-4022-8c78-3da7db8e3f70)

2. Clock requency settings remained unchanged:
![image](https://github.com/user-attachments/assets/ed4481f1-5d87-482e-a145-f523068fb3bb)

3. Adjustement for using floating point computations on the FFT ip itself:
![image](https://github.com/user-attachments/assets/8063ab18-385f-48eb-a745-17fac74c96cd)


## Other useful things
This sample implement float-based approach to that:
* https://github.com/DYGV/HLS_FFT
* https://www.youtube.com/watch?v=HR4h_T4HZB0&ab_channel=FPGAPS - FPGA PS approach with PYNQ framework
* https://youtu.be/aySO9jCKj9g - ZYNQ DMA tutorial
* https://www.youtube.com/@BRH_SoC - Really cool channel with a huge amount of other resources regarding Xilinx SoC
