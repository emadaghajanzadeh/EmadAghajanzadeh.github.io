---
title: "Kmeans Parallelism with OpenMp & Cuda"
collection: project
image: "/images/Parallelism.png"
keywords: "Parallel Computing - GPU Computing - CPU Parallelism"
description: "The aim of this project was to implement the theories that were taught during the course of multi-core programming. The task was to improve the execution time of the Kmeans algorithm by dividing its computational loads first among the CPU cores and second among GPU blocks. To do this, each data point was considered as a single processing thread, in which its distance from the cluster center was computed. In the end, the results of the threads were merged by the main thread, and clusters were updated based on these calculations. To compare the methods, compressed representations of the MNIST dataset images, obtained by a trained CNN, were used. Finally, the execution time of the openMP approach was only half of the serial one, but the speed up for the GPU approach was far better, its execution time was one-ninth of the serial one. This shows the capability of GPUs for optimizing the problems which can be divided into some smaller problems, all of which do exactly the same task. (if tasks were different, the performance of GPU could not be better than CPU)"
---
