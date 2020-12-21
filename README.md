# Image-Compression


Objective: You are an engineer in Shutterstock and responsible for optimizing the web experience on the site. You will serve images that exhibit minimal distortion at the best possible storage efficiency. You need to come up with a python implementation that takes images in and compresses them to satisfy the above requirements.  
### First you need to persuade yourself that you know the basics and you may find [this](http://www.eecs.umich.edu/courses/eecs206/archive/fall03/public/lab/lab5/lab5.pdf) useful. 

### 1. You assume that the segment/block size used in the compression scheme is 8x8, and the DCT coefficients (64 of them) are “independent” Gaussian sources. Your main task is to evaluate the R(D) function of the DCT-transformed image using this independent (yet non-identical) assumption. In the process of evaluating the R(D) function, you will perform (virtually) no quantization (except for simple rounding off of the DCT coefficients to nearest integers as needed). Treat each of the 64 coefficients as an independent Gaussian source with its own variance. Evaluate the variances $\sigma^2_i, i=1,2,...64$ of the DCT coefficients. Plot the variances as a function of the DCT coefficient index (from 1 to 64). Use Zig-Zag scanning order to identify the DCT coefficient indices. (5 points) 
### 2.  Find the maximum variance σ^{max} among the above DCT variances. This maximum variance $σ^2_{max}$ can simply be used to define an adequate range of distortion values. For example, D=range(10**-4, 1.0, 10**-4)*sigma_max^2. (5 points) 
### 3.  Evaluate the individual R(D) functions R_i(D), i=1, 2,...,64 for the DCT coefficients (as a function of the distortion values D). Plot all RD functions (64 of them) in a single figure. What observations can you make about the RD functions? Plot all RD functions of the AC coefficients (63 of them), mainly to get an insight into the AC R(D) functions in isolation of the DC R(D) function. (10 points) Implement a DCT transform compressor in python that consists of a DCT transformer, a Quantizer and an encoder of your choice. The compressor takes as input images [from the gray-scale sets 1 and 2](http://links.uwaterloo.ca/Repository.html) and optimizes the rate according to the tradeoff between rate R and distortion D (D + lambda * R) where lambda is the Langrange multiplier, as described in [this](https://engineering.purdue.edu/~zhu0/ece634_s19/lecture/rd-ortega-spm1998.pdf) paper. You can use any optimization library in python you need eg.[CVXPY](https://www.cvxpy.org/related_projects/index.html).  (30 points)


This project was created with support of: 
*   [Zigzag-Scan](https://github.com/asad82/Zigzag-Scan) By asad82
*   [compression-DCT](https://github.com/getsanjeev/compression-DCT) By getsanjeev
*   [ImageCompression](https://github.com/faizanayubi/ImageCompression) By faizanayubi

*   [dct-image-compression](https://github.com/samueldemoura/dct-image-compression) By samueldemoura
*   [simple-JPEG-compression](https://github.com/amzhang1/simple-JPEG-compression) By amzhang1
*   [Images, Compression, and Coding](http://www.eecs.umich.edu/courses/eecs206/archive/fall03/public/lab/lab5/lab5.pdf) By EECS at Michigan
*   Zigzag *Scanner* Created By Alexey S. Sokolov a.k.a. nICKEL, Moscow, Russia


This Project was done on Google Colab [here](https://colab.research.google.com/drive/1w6TkOMRWUccEYwQZHXYDsNFR_049RSRu?usp=sharing).
Remark: There are some logical errors in the code as I am a novice in Python. 



