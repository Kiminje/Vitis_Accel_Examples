Clock Frequency ~ Large Loop Count (C)
======================

This is a CNN (Convolutional Neural Network) based example which mainly focuses on Convolution operation of a CNN network. The goal of this example is to demonstrate a method to overcome kernel design timing failure issue. It also presents the effectiveness of using multiple compute units to improve performance.

***KEY CONCEPTS:*** Clock Frequency, Multiple Compute Units, Convolutional Neural Networks

***KEYWORDS:*** #pragma HLS ARRAY_PARTITION, #pragma HLS PIPELINE, #pragma HLS INLINE

## SUPPORTED PLATFORMS
Platform | Board             | Software Version
---------|-------------------|-----------------
xilinx_aws-vu9p-f1-04261818|Xilinx Only 5.0 Shell|SCOUT 2019.1
xilinx_u200_qdma|Xilinx Alveo U200|SCOUT 2019.1
xilinx_u280_xdma|Xilinx Alveo U280|SCOUT 2019.1
xilinx_u250_qdma|Xilinx Alveo U250|SCOUT 2019.1
xilinx_u200_xdma|Xilinx Alveo U200|SCOUT 2019.1
xilinx_u250_xdma|Xilinx Alveo U250|SCOUT 2019.1
xilinx_u280-es1_xdma|Xilinx Alveo U280|SCOUT 2019.1


##  DESIGN FILES
Application code is located in the src directory. Accelerator binary files will be compiled to the xclbin directory. The xclbin directory is required by the Makefile and its contents will be filled during compilation. A listing of all the files in this example is shown below

```
src/cnn_convolution.cpp
src/cnn_convolution_bad.cpp
src/defns.h
src/host.cpp
```

##  COMMAND LINE ARGUMENTS
Once the environment has been configured, the application can be executed by
```
./host <cnn_GOOD XCLBIN> <cnn_BAD XCLBIN>
```
