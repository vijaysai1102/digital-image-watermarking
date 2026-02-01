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

```
Digital-Watermarking-main/
├── Code/
│   ├── watermark_generator.py
│   │   └── Embeds a watermark into the original image using XOR operations
│   │       and random point selection for secure embedding
│   │
│   ├── master_share_generator.py
│   │   └── Generates master shares for watermark verification by creating
│   │       secure shares based on image gradients and thresholding
│   │
│   ├── owernership_share_generator.py
│   │   └── Extracts ownership-related watermark data and generates
│   │       ownership verification shares
│   │
│   └── template_match_res.py
│       └── Performs template matching to verify watermark presence in
│           stolen, modified, or regenerated images
│
├── images/
│   ├── master_images/
│   │   └── Original images used for watermarking
│   │
│   ├── stolen_images/
│   │   └── Simulated stolen/modified images for testing
│   │
│   └── regenerated_watermarks/
│       └── Extracted and regenerated watermarks from stolen images
│
├── README.md
│   └── Project documentation and usage guide
│
└── .gitignore
    └── Git ignore configuration
```

### Key Components

| Component | Purpose | Input | Output |
|-----------|---------|-------|--------|
| **Watermark Generator** | Embeds watermark into images | Original image, Watermark data | Watermarked image |
| **Master Share Generator** | Creates verification shares | Watermarked image | Master shares |
| **Ownership Share Generator** | Extracts ownership data | Watermarked image | Ownership shares |
| **Template Matcher** | Verifies ownership | Stolen image, Template | Matching confidence score |

---

## How to Run

### Prerequisites
```bash
pip install opencv-python numpy matplotlib
