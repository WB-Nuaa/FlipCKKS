# FlipCKKS: Bit-Level Sensitivity Analysis for Data Integrity and Communication Optimization in CKKS

FlipCKKS allows controlled fault injection (i.e., bit flips) during FHE evaluation operations, aiming to minimize the mean squared error (MSE) of the decrypted ciphertext relative to that obtained without fault injection.
In this repository, we provide the source code, configuration files, requirements, and partial data.
 
## Setup
FlipCKKS is developed upon the C++ Microsoft SEAL library (version 4.1.2). Therefore, you need to install a matching version of SEAL first, then compile FlipCKKS.

### Build and Install Microsoft SEAL
In the Ubuntu system, open the terminal and execute the following commands:
```bash
git clone  https://github.com/microsoft/SEAL.git
cd SEAL

# Configure the build
cmake -S . -B build
cmake --build build

# Install to the system
sudo cmake --install build
```

### Install FlipCKKS
After creating the `CKKS` folder inside the SEAL `native` directory and copying all files into it. Then, open the terminal and execute the following commands:
```bash
sudo cmake -S . -B build
sudo cmake --build build
```
This way, an executable file named CKKS can be obtained:
```bash
 cd build/bin
 ./CKKS
```


