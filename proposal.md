# B657 Final Project Proposal

## Project Title

Active Learning for Efficient Flood Inundation Mapping

## Team Members
Aolong Li, Yevhen Melnyk, Sean Dixit, Vishakha Dikshit

## Project Description

This project aims to explore active learning techniques to significantly speed up the data annotation process for flood inundation mapping from satellite imagery. The primary goal is to integrate an active learning approach into an existing browser-based annotation software developed by the project team. This approach will recommend the most effective superpixels in an image for users to annotate, reducing the number of pixels that need to be manually annotated and minimizing the uncertainty of the underlying machine learning model for flood area segmentation.

The project will involve conducting human-model interactions to study and compare the effectiveness of different acquisition functions in the active learning framework. The acquisition functions will be designed based on prediction uncertainty, prediction consistency/robustness to input data augmentation, and temporal output discrepancy during model training. The project will also explore the possibility of replacing the current U-Net backbone for flood pixel segmentation with more advanced models, such as the recent transformer-based geo-foundation model Prithvi, to improve the segmentation performance.

## Reading List


- Few-Shot Adaptive Gating for Single-Step Unsupervised Domain Adaptation" (https://arxiv.org/abs/2112.07805) - relevant for potential integration of transformer-based models
- Prithvi: A Geo-Foundation Model for Multilingual and Multimodal Earth Observation (https://arxiv.org/abs/2303.16970) - the transformer-based geo-foundation model to be explored
- Learnable Visual Prompts for Incremental Learning (https://arxiv.org/abs/2203.12119) - visual prompt tuning technique for efficient model adaptation
- LoRA: Low-Rank Adaptation of Large Language Models (https://arxiv.org/abs/2106.09685) - LoRA technique for efficient model adaptation

## Research Plan and Timeline

- March 11 - March 18: Familiarize with the existing annotation software and active learning framework. Understand the current acquisition functions and the U-Net backbone.
- March 18 - Apr 1: Implement and integrate new acquisition functions based on prediction uncertainty, consistency, and temporal discrepancy. Conduct human-model interactions to evaluate the effectiveness of different acquisition functions. Also, prepare interim project presentation.
- Apr 1 - Apr 15: Explore the integration of the Prithvi transformer-based model as a replacement for the U-Net backbone. Investigate techniques like LoRA and visual prompt tuning for efficient model adaptation.
- Apr 15 - Apr 28: Prepare the project poster, finalize the active learning framework, conduct final experiments, and prepare the project report.

Rather than dividing up the work, we plan to engage in the work collaboratively. Should the need arise, we may opt to distribute responsibilities accordingly.

## Plan for Data and Experiments

The project will utilize the existing high-resolution optical imagery and digital elevation model (DEM) data collected by the project team. The effectiveness of the active learning approach will be measured by the reduction in the number of pixels that users need to annotate while maintaining or improving the accuracy of flood area segmentation compared to the current manual annotation process.

The experiments will involve running the active learning framework with different acquisition functions and evaluating their performance in terms of annotation efficiency and segmentation accuracy. The final experiments will also include evaluating the performance of the integrated Prithvi model or other advanced models compared to the current U-Net backbone.

A subset of the available dataset will be used for initial experimentation and development, while the full dataset will be employed for final evaluation and comparison with the baseline manual annotation approach.
