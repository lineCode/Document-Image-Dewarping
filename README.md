![equation](http://latex.codecogs.com/gif.latex?%5Cpsi%28x%29%20%3D%20%5Cbegin%7Bcases%7D%20x%5E2%20%26%20%5Ctext%7Bif%7D%7E%7Cx%7C%5Cleq%201%5C%5C%202%7Cx%7C-1%20%26%5Cmathrm%7Bif%7D%7E%20%7Cx%7C%20%3E%201%5Cend%7Bcases%7D)

# Robust Document Image Dewarping Method using Text-lines and Line Segments (ICDAR 2017)


<p align="center">
<img src="/images/abs.png" width="800"> 
</p>


## Abstract
Conventional text-line based document dewarping
methods have problems when handling complex layout and/or
very few text-lines. When there are few aligned text-lines in the
image, this usually means that photos, graphics and/or tables take
large portion of the input instead. Hence, for the robust document
dewarping, we propose to use line segments in the image in
addition to the aligned text-lines. Based on the assumption and
observation that many of the line segments in the image are
horizontally or vertically aligned in the well-rectified images,
we encode this property into the cost function in addition to
the text-line alignment cost. By minimizing the function, we can
obtain transformation parameters for camera pose, page curve,
etc., which are used for document rectification. Considering that
there are many outliers in line segment directions and missed
text-lines in some cases, the overall algorithm is designed in an
iterative manner. At each step, we remove text components and
line segments that are not well aligned, and then minimize the
cost function with the updated information. Experimental results
show that the proposed method is robust to the variety of page
layouts.


## Algorithm
### Proposed cost function
For the parametric modeling of the dewarping process, we adopt the model in [1].
By this model, the geometric relation between the captured image domain and the rectified document domain can be
parameterized with the polynomial parameters and camera pose matrix.
For the estimation of these dewarping parameters, we develop a cost function:

where $ E=mc^2 $


### Alignments of line semgents and its term
### Outlier removal and optimization


## Experimental results
### Experimental results on CBDAR 2007 dewarping contest dataset
### Experimental results on our dataset (non conventional images)


## Reference
