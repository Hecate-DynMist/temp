# Abstract
Unlike images which are represented in regular dense
grids, 3D point clouds are irregular and unordered, hence
applying convolution on them can be difficult. In this paper,
we extend the dynamic filter to a new convolution operation, named PointConv. PointConv can be applied on point
clouds to build deep convolutional networks. We treat convolution kernels as nonlinear functions of the local coordinates of 3D points comprised of weight and density functions. With respect to a given point, the weight functions
are learned with multi-layer perceptron networks and density functions through kernel density estimation. The most
important contribution of this work is a novel reformulation proposed for efficiently computing the weight functions,
which allowed us to dramatically scale up the network and
significantly improve its performance. The learned convolution kernel can be used to compute translation-invariant
and permutation-invariant convolution on any point set in
the 3D space. Besides, PointConv can also be used as deconvolution operators to propagate features from a subsampled point cloud back to its original resolution. Experiments
on ModelNet40, ShapeNet, and ScanNet show that deep
convolutional neural networks built on PointConv are able
to achieve state-of-the-art on challenging semantic segmentation benchmarks on 3D point clouds. Besides, our experiments converting CIFAR-10 into a point cloud showed that
networks built on PointConv can match the performance of
convolutional networks in 2D images of a similar structure.
