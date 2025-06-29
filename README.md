# Steel-Slag-Concrete-Datasets
This repository provides a curated dataset for the study of instance segmentation and homogeneity evaluation of aggregates in steel slag concrete. The dataset was developed to support research in intelligent concrete quality inspection, particularly in the context of aggregate composition analysis and slag substitution rate evaluation.
Dataset Description
The dataset includes 1,784 high-resolution images of cut cross-sections of steel slag concrete specimens with varying substitution ratios of natural aggregate by steel slag. Specimens were prepared based on volume replacement of coarse aggregates following the Chinese national standard JGJ 55-2011: Design Code for Ordinary Concrete Mix Proportion, and include the following substitution ratios: 0%, 10%, 20%, ..., up to 100%. Each ratio group contains 20 concrete specimens, resulting in 11 groups in total.

Concrete Mix Design (per m³)
Substitution Rate	Natural Sand	Natural Aggregate	Steel Slag Aggregate	Cement	Water
1	0	770.13	1020.87	0	435	174
2	10	770.13	918.783	102.087	435	174
3	20	770.13	816.696	204.174	435	174
4	30	770.13	714.609	306.261	435	174
5	40	770.13	612.522	408.348	435	174
6	50	770.13	510.435	510.435	435	174
7	60	770.13	408.348	612.522	435	174
8	70	770.13	306.261	714.609	435	174
9	80	770.13	204.174	816.696	435	174
10	90	770.13	102.087	918.783	435	174
11	100	770.13	0	1020.87	435	174


Image Acquisition and Annotation
After standard curing, each concrete specimen was vertically sliced to expose internal aggregate distributions. A custom imaging setup was designed to ensure consistent lighting and high-contrast image capture. The acquired raw images were augmented using cropping, rotation, and salt-and-pepper noise addition.


For semantic segmentation tasks, all images were pixel-wise annotated using the AnyLabeling software. Three classes were labeled: natural aggregate, steel slag aggregate, and pores. Unlabeled or ambiguous regions were marked as background. To improve annotation efficiency and segmentation detail, the Segment Anything Model (SAM) developed by Meta AI was integrated into the annotation process.

A visual comparison between traditional manual annotation and SAM-assisted annotation is shown below:

Traditional Annotation	SAM-assisted Annotation

Dataset download link： 
![image](https://github.com/user-attachments/assets/28bb97d6-7635-4b3c-b789-14202f6db625)


Intended Use
This dataset is intended for academic and research purposes in the fields of:

Semantic and instance segmentation

Material classification in concrete

AI-assisted concrete quality inspection

Steel slag utilization and performance analysis

Contact
For collaboration or questions, please contact:
Shangjun Zhao
PhD Student, Hainan University
Email: zhaoshangjun@foxmail.com
