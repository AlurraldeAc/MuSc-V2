# MuSc-V2

**This is an official PyTorch implementation for "MuSc-V2: Zero-Shot Multimodal Industrial Anomaly Classification and Segmentation with Mutual Scoring of Unlabeled Samples"**

Authors:  [Xurui Li](https://github.com/xrli-U)<sup>1</sup> | [Feng Xue](https://xuefeng-cvr.github.io/)<sup>3</sup> | [Yu Zhou](https://github.com/zhouyu-hust)<sup>1,2</sup>

Institutions: <sup>1</sup>Huazhong University of Science and Technology | <sup>2</sup>Wuhan JingCe Electronic Group Co.,LTD | <sup>3</sup>University of Trento

### 🧐 [Arxiv](https://arxiv.org/abs/2511.10047)

## TODO

Our manuscript is currently under review. We plan to make the complete code repository public upon its acceptance.

The previous version, i.e. **[MuSc](https://arxiv.org/pdf/2401.16753.pdf)** is published in ICLR-2024 **([github](https://github.com/xrli-U/MuSc))**

## 👇Abstract

Zero-shot anomaly classification (AC) and segmentation (AS) methods aim to identify and outline defects without using any labeled samples. In this paper, we reveal a key property that is overlooked by existing methods: normal image patches across industrial products typically find many other similar patches, not only in 2D appearance but also in 3D shapes, while anomalies remain diverse and isolated.

To explicitly leverage this discriminative property, we propose a Mutual Scoring framework (MuSc-V2) for zero-shot AC/AS, which flexibly supports single 2D/3D or multimodality. Specifically, our method begins by improving 3D representation through Iterative Point Grouping (IPG), which reduces false positives from discontinuous surfaces. Then we use Similarity Neighborhood Aggregation with Multi-Degrees (SNAMD) to fuse 2D/3D neighborhood cues into more discriminative multi-scale patch features for mutual scoring. The core comprises a Mutual Scoring Mechanism (MSM) that lets samples within each modality to assign score to each other, and Cross-modal Anomaly Enhancement (CAE) that fuses 2D and 3D scores to recover modality-specific missing anomalies. Finally, Re-scoring with Constrained Neighborhood (RsCon) suppresses false classification based on similarity to more representative samples.

Our framework flexibly works on both the full dataset and smaller subsets with consistently robust performance, ensuring seamless adaptability across diverse product lines. In aid of the novel framework, MuSc-V2 achieves significant performance improvements: a $\textbf{+23.7\%}$ AP gain on the MVTec 3D-AD dataset and a $\textbf{+19.3\%}$ boost on the Eyecandies dataset, surpassing previous zero-shot benchmarks and even outperforming most few-shot methods.

## Citation:
```
@inproceedings{arxiv2025MuScV2,
  title={MuSc-V2: Zero-Shot Multimodal Industrial Anomaly Classification and Segmentation with Mutual Scoring of Unlabeled Samples},
  author={Li, Xurui and Xue, Feng and Zhou, Yu},
  journal={arXiv preprint arXiv:2511.10047},
  year={2025}
}
```

## License:
MuSc-V2 is released under the **MIT Licence**, and is fully open for academic research and also allow free commercial usage. To apply for a commercial license, please contact yuzhou@hust.edu.cn.
