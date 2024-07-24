# Classification of Remote Image Sensing Dataset using Partial Cross Entropy
## Dataset:
DeepGlobe Land Cover Classification, consisting of 7 classes of Land.
## Partial Cross Entropy Loss Function:
Partial Cross Entropy (PCE) improves image segmentation, especially for remote sensing images, by addressing the limitations of standard Cross Entropy (CE). In remote sensing, images often contain vast amounts of background or irrelevant data, making precise segmentation challenging. CE calculates loss over the entire image, including less relevant regions, potentially diluting the focus on crucial segmentation areas. PCE, however, selectively focuses on more informative pixels or regions, enhancing the model's ability to learn from the most relevant parts of the image. This selective approach helps mitigate the imbalance between foreground and background, leading to more accurate and efficient segmentation outcomes, which is particularly beneficial for the complex and detailed nature of remote sensing imagery.
## Architecture:
**U-Net** was used for classficiation as it good for tasks involving masking and satellite image data due to its effectiveness in semantic segmentation, which is the process of classifying each pixel in an image into a specific class.  
**Deep U-Nets** increase the number of parameters thus improving the performance of the model as deeper models tend to learn better than shallow networks.  
**Multi-Scale Feature Fusion:** 
Multi-Scale Feature Fusion is a technique used to enhance the performance of neural networks.  
- Feature Extraction at Multiple Scales: The network extracts features at different resolutions or scales using various branches or pathways. These branches can be created by applying different pooling or dilated convolution operations.
- Fusion of Features: The features extracted at these different scales are then combined, typically by concatenation or summation, to produce a comprehensive representation that includes both local and global context.
