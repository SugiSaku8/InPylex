# InPylex Power Engine - GPUCL Module

## Overview

This document provides an overview of the `gpuCL.js` module, part of the InPylex Power Engine developed by Carnation Games. The module leverages the GPU.js library to perform matrix operations on the GPU, offering a powerful tool for game development and other applications requiring high-performance matrix computations.

## Features

- **Matrix Operations**: The module supports basic matrix operations such as addition, subtraction, multiplication, and division.
- **GPU Acceleration**: Utilizes the GPU.js library to perform these operations on the GPU, significantly improving performance for large matrices.
- **Custom Kernel Creation**: Allows for the creation of custom kernels for specific matrix operations, offering flexibility and optimization.

## Getting Started

### Prerequisites

- Node.js installed on your system.
- The `gpu.js` library installed via npm: `npm install gpu.js`.

### Installation

1. Clone the repository or download the `gpuCL.js` file.
2. Install the `gpu.js` library by running `npm install gpu.js` in your project directory.

### Usage

To use the `gpuCL` module in your project, first, import it:

javascript const { GPUCL } = require('./gpuCL');


Then, create an instance of the `GPUCL` class:

javascript const gpuCL = new GPUCL();


You can now perform matrix operations using the methods provided by the `GPUCL` class:

javascript // Example: Matrix multiplication const result = gpuCL.multiply(matrixA, matrixB);

// Example: Matrix addition const sum = gpuCL.add(matrixA, matrixB);

// Example: Matrix subtraction const difference = gpuCL.subtract(matrixA, matrixB);

// Example: Matrix division const quotient = gpuCL.divide(matrixA, matrixB);


### Custom Kernel Creation

For more complex operations or optimizations, you can create custom kernels using the `createKernel` method of the `GPU` instance:

javascript const customKernel = gpu.createKernel(function(a, b) { // Custom operation logic here }).setOutput([512, 512]);


## Contributing

Contributions to the InPylex Power Engine are welcome. Please follow the standard GitHub workflow: fork, branch, commit, and pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## Contact

For any questions or support, please contact Carnation Games at support@carnationgames.com.