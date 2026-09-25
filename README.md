# CUDA Sobel Edge Detection Capstone

## Description

This project implements Sobel edge detection for RGB PPM images using both a CPU
baseline and a CUDA GPU kernel. It demonstrates:

- GPU kernel design with one thread per output pixel.
- RGB-to-grayscale conversion on the fly.
- 3x3 Sobel convolution with boundary clamping.
- CPU/GPU result verification.
- Command-line interface with configurable block size.
- Timing and proof-of-execution support.

The GPU version is intended to show how a regular image-processing operation can
be parallelized across many threads and compared against a correct CPU reference.

## Requirements

- NVIDIA GPU with CUDA support.
- CUDA Toolkit 11.0 or newer.
- C++17 compiler.
- Python 3 only for generating the sample PPM image.

## Build

```bash
make clean
make
