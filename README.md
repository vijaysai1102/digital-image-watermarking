# Digital Image Watermarking for Copyright Protection

## Overview
This project implements a digital image watermarking system designed for copyright protection and ownership verification. A watermark is embedded into an original image, ownership information is split into multiple shares, and template matching techniques are used to verify ownership even if the image is stolen or modified.

The project demonstrates concepts from digital image processing, security, and multimedia authentication.

---

## Features
- Watermark embedding into digital images
- Master and ownership share generation
- Reconstruction of watermark from modified or stolen images
- Ownership verification using template matching
- Simulation of copyright infringement scenarios

---

## Tools & Technologies
- **Python**
- **OpenCV**
- **NumPy**
- **Matplotlib**

---

## Project Structure
- **Watermark Generation:** Embeds watermark into the original image
- **Master Share Generation:** Creates secure master shares for verification
- **Ownership Share Generation:** Extracts ownership-related watermark data
- **Template Matching:** Verifies watermark presence in stolen or altered images
- **Image Assets:** Stores original, watermarked, stolen, and regenerated images

---

## How to Run

### Prerequisites
```bash
pip install opencv-python numpy matplotlib
