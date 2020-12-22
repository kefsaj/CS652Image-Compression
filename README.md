#Image-Compression

You are an engineer in Shutterstock and responsible for optimizing the web experience on the site. You will serve images that exhibit minimal distortion at the best possible storage efficiency. You need to come up with a python implementation that takes images in and compresses them to satisfy the requirements found [here](https://github.com/kefsaj/CS652Image-Compression).

Full Requirements can be found [here](

In this project, there are many components which include

1.  Reading the image
2.  Transforming the image into blocks
3.  Performing Discrete Cosine Transformation
4.  Quantizing Dct which saves the approximations and omit details
5.  Showing how you can save a DCT block aas small as it can be by Zig-Zag, Huffman Coding and Run-length Encoding
6.  The image is saved back into a JPEG file
7.  Decoding the using Run-Length decoding, Zig-Zag decding and huffman decoding 
8.  Decompression of the encoded image
9.  Finding the Rate Distortion of the image

Items to get sorted: 
-  R(D) Plot
-  Simplifying R(D) plotting code
-  Implementing of optimizing the rate according to the tradeoff between rate R and distortion D (D + lambda * R) where lambda is the Langrange multiplier

This project was created with support of: 
*   [Zigzag-Scan](https://github.com/asad82/Zigzag-Scan) By asad82
*   [compression-DCT](https://github.com/getsanjeev/compression-DCT) By getsanjeev
*   [ImageCompression](https://github.com/faizanayubi/ImageCompression) By faizanayubi
*   [dct-image-compression](https://github.com/samueldemoura/dct-image-compression) By samueldemoura
*   [simple-JPEG-compression](https://github.com/amzhang1/simple-JPEG-compression) By amzhang1
*   [Images, Compression, and Coding](http://www.eecs.umich.edu/courses/eecs206/archive/fall03/public/lab/lab5/lab5.pdf)
*   [JPEG-DCT-Compression](https://github.com/timmmGZ/JPEG-DCT-Compression/blob/master/JpegCompression.ipynb) By timmmGZ
*   [PyRate](http://tuvalu.santafe.edu/~simon/styled-13/) By Simon DeDeo

Please do note this is compliation of code from various sources mentioned above.

Image used: [raccoon-procyon-lotor.jpg](http://www.public-domain-image.com/)

Key Terms:
*  A discrete cosine transform (DCT) expresses a finite sequence of data points in terms of a sum of cosine functions oscillating at different frequencies.
*  Rate–distortion theory is a major branch of information theory which provides the theoretical foundations for lossy data compression; it addresses the problem of determining the minimal number of bits per symbol, as measured by the rate R, that should be communicated over a channel, so that the source (input signal) can be approximately reconstructed at the receiver (output signal) without exceeding an expected distortion D.

This Project was done on Google Colab [here](https://colab.research.google.com/drive/1w6TkOMRWUccEYwQZHXYDsNFR_049RSRu?usp=sharing).
Remark: There are some logical errors in the code as I am a novice in Python. 



