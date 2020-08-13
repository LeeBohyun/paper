# Ozone (O3): An Out-of-Order Flash Memory Controller Architecture Paper Analysis

**:warning: for personal study only**

## 0. Abstract
**Ozone(O3)** is flash memory controller capable of executing multiple flash operations out of order. Execution of multiple flash operations in O3 flash controller are constrained by data order, thus making multichip parallelism a better option than memory interleaving. O3 controlller provides prioritized handling of flash operations by using FTL. By testing workloads on an FPGA implementation, O3 controller achieved  33 percent higher throughput and 50 percent lower response time compared to interleaving.

## 1. Introduction

In order to present same storage interface as an HDD and overcome limitation if flash memory, FTL Is used in flash storage devices. Efficient FTL exploit multiple concurrent flash chips essentially 
