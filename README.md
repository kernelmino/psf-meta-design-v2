PSF-Engineered Meta-Optics in TensorFlow
This repository contains a Google Colab notebook for designing RGB meta-optics that produce customized point spread functions (PSFs) using TensorFlow.
Summary
- Simulates meta-optics that generate 7×7 RGB kernels, inspired by convolutional filters from CIFAR-10.
- Each kernel is split into positive and negative components to ensure physical realizability.
- Silicon nitride pillar structures are modeled and optimized for 450, 532, and 635 nm wavelengths.
- A differentiable proxy models the phase shift from pillar width, enabling gradient-based optimization.
- The angular spectrum method simulates light propagation to match optical PSFs with targets.
- The loss function minimizes RMS errors across RGB channels using the Adam optimizer.
Included
- TF_for_PSF_Engineering_CIFAR.ipynb: Complete pipeline for metasurface simulation and optimization.
Requirements
- Google Colab
- TensorFlow
- NumPy, SciPy, Matplotlib
License
This project is released under the MIT License.
