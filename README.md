# IP-QIR



Intensity-Preserving Quantum Image Representation (IP-QIR)



---


 Description

IP-QIR is a hybrid quantum image representation technique that focuses on preserving pixel intensity while minimizing qubit usage and circuit depth. This project implements IP-QIR using Qiskit, allowing efficient quantum image encoding and simulation.  



The project is applicable to:

Synthetic images

SAR images

Medical images



---


 Features

 Resource-efficient quantum image encoding

Accurate pixel intensity preservation

 Simulation using Qiskit

 Supports grayscale image patches



---



# Workflow

1\. Image Input 

&nbsp;  Load synthetic, SAR, or medical image patches.



2\. Preprocessing

&nbsp;  - Resize images to \\(2^n \\times 2^n\\)  

&nbsp;  - Normalize pixel intensities to \\(\[0,1]\\)



3\. Pixel-to-Angle Mapping

&nbsp;  Compute \\(\\theta\_{x,y} = 2 \\cdot \\arccos(pI\_{x,y})\\) for each pixel.



4\. Quantum Encoding (IP-QIR)

&nbsp;  - Assign position qubits and intensity qubit

&nbsp;  - Apply Controlled Ry (θ) gates

&nbsp;  - Construct quantum circuit in Qiskit



5\. Simulation  

&nbsp;  - Run the quantum circuit on Qiskit simulator  

&nbsp;  - Evaluate intensity preservation and fidelity



---



# Installation

1\. Clone the repository:

```bash

git clone https://github.com/poojadhingiya/IP-QIR.git


pip install qiskit matplotlib numpy


