# Setup-NVIDIA-GPU-for-Deep-Learning
Step 1: Install NVIDIA Video Driver

Download and install the latest NVIDIA GPU driver from the official source:

NVIDIA GPU Driver Download

Step 2: Install Visual Studio C++

Visual Studio with C++ support is required. By default, C++ is not installed, so ensure you select all relevant C++ options.

Download Visual Studio Community Edition

Step 3: Install Anaconda/Miniconda

Anaconda or Miniconda is needed to manage dependencies and install deep learning packages.

Download Anaconda

Step 4: Install CUDA Toolkit

CUDA is required for GPU-accelerated computations.

Download CUDA Toolkit

Step 5: Install cuDNN

cuDNN is a GPU-accelerated library for deep learning.

Download cuDNN

Step 6: Install PyTorch

Follow the official PyTorch installation guide to install PyTorch with CUDA support.

Install PyTorch

Step 7: Verify Installation

Run the following Python script to verify that your GPU is detected and being used:
import torch

print("Number of GPU: ", torch.cuda.device_count())
print("GPU Name: ", torch.cuda.get_device_name())


device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
print('Using device:', device)
