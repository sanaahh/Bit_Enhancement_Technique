PROJECT TITLE: “Learning to Generate Realistic Images for Bit-Depth Conversion using RealGAN”
 
 
SUBMITTED BY :
23MIA1028-ANJUM SANA
23MIA1090-THARUNIKA RAVI KUMAR
23MIA1092-A.JAI AAKAASH

 
ABSTRACT:
Digital images captured by modern cameras are often stored in high bit-depth formats such as 16-bit to preserve fine tonal details and dynamic range. However, most display systems and social media platforms operate with 8-bit images, which leads to a reduction in color precision and visible loss of quality when converting from 16-bit to 8-bit. This project focuses on simulating this bit-depth conversion process and restoring the visual realism of the degraded images using a Generative Adversarial Network (RealGAN).
The RealGAN framework is used to generate realistic 8-bit representations by mimicking the behavior of camera imaging pipelines. The system first performs quantization to reduce the image depth from 16-bit to 8-bit, introducing controlled tone and color losses. Then, enhancement techniques inspired by RealGAN, such as tone mapping, contrast stretching, and detail enhancement, are applied to produce visually pleasing results. Experimental observations show that the proposed approach can generate 8-bit images that retain natural appearance and fine details, effectively simulating real-world photographic outputs.
This project demonstrates the effectiveness of RealGAN-based image processing in learning realistic transformations between different bit-depths, which can be further extended for bit-depth enhancement tasks and camera image optimization

BASE PAPER REFERENCE:

J. Liu, W. Zou, H. Zhao, and Y. Zhou, “Learning to Generate Realistic Images for Bit-Depth Enhancement via Camera Imaging Processing,” IEEE Transactions on Image Processing, vol. 32, pp. 1044–1056, 2023.

TOOLS AND LIBRARIES USED:

Framework: PyTorch

Libraries: NumPy, OpenCV, Matplotlib, Scikit-Image, PIL

Environment: Python 3.9, CUDA-enabled GPU

STEPS TO EXECUTE THE CODE:

Install dependencies using pip install -r requirements.txt.

Load the training dataset (e.g., MIT-Adobe 5K).

Run train.py to train the RealGAN model.

Execute test.py to generate enhanced images.

Evaluate results using quality metrics (NIMA, NIQE, PIQE, BRISQUE).

DESCRIPTION OF DATASET:

MIT-Adobe 5K: 5,000 professional 16-bit RAW images for generating synthetic low-bit-depth pairs.

DPED: 22,000 smartphone and DSLR 8-bit image pairs for real-world evaluation.

HDR Dataset: Used for 16-bit reference comparison.

OUTPUT / RESULT SUMMARY:

RealGAN-trained models achieved NIMA = 6.81, improving over 6.35 without RealGAN.<img width="1732" height="656" alt="image" src="https://github.com/user-attachments/assets/0a158bfd-3bf9-474b-a112-f7f3aa6b41ca" />


Significant reductions observed in NIQE, PIQE, and BRISQUE values.

YOUTUBE DEMO LINK:
https://www.youtube.com/watch?v=WCvesSrsvYQ&feature=youtu.be

Visual results show smoother gradients, sharper textures, and reduced banding artifacts compared to baseline models.
