# A Survey on IQA: Insights, Analysis, and Future Outlook

![img1](assets/Metric_Struct.jpg)

## 🔍 Introduction

Image Quality Assessment (IQA) is a critical component of image-related technologies and plays a pivotal role in the advancement of image processing and computer vision. In recent years, the proliferation of novel training frameworks and machine learning models has given rise to a multitude of IQA methodologies. This survey conducts a comprehensive review of nearly 200 IQA-related publications, synthesizing key developments in the field and systematically categorizing existing approaches based on their underlying models, training frameworks, publication timelines, application scenarios, and academic impact. This structured analysis aims to facilitate a swift introduction for newcomers while providing seasoned researchers with a clearer perspective on the current state of the field. Moreover, we offer a critical evaluation of the advantages and limitations of various IQA methods and present our perspectives on future research directions. To complement the survey, this repository compiles both the IQA techniques discussed in the paper and other approaches that could not be included due to space constraints, thereby serving as a valuable resource to support further advancements in IQA research.<br>

图像质量评估（IQA）在图像相关的技术中起着非常重要的作用，对于图像处理和计算机视觉领域的技术发展有着深远的影响。近年来，随着新型训练框架和机器学习模型的出现，许多IQA方法涌现出来。本综述通过调研接近二百篇IQA相关论文，总结了IQA发展中值得关注的工作，并按照不同方法所用的模型、训练框架、发表时间、使用场景和影响力进行了整理，以方便初学者快速入门、资深研究者更好地了解领域发展现状。随后，我们对诸多IQA方法的优缺点进行了分析，对IQA方法的未来发展提出了自己的见解。本repository旨在列出论文中提到的、以及受篇幅限制未提到的经典IQA方法，配合论文阅读，以促进IQA技术的发展。

🚀English Paper link: [A Survey on Image Quality Assessment: Insights, Analysis, and Future Outlook](https://arxiv.org/abs/2502.08540)<br>
🚀Chinese Paper link: [在计算机视觉领域中，我们应该如何评估图像质量（万字长文）？](https://zhuanlan.zhihu.com/p/25680975953)

## Update Records

- 🔥 [March.2,2025] The chinese version of our survey has been released on zhihu.
- 🔥 [Feb.12,2025] The first version of our survey has been released on arXiv.

## 📜 Table of Contents

📚 Image Quality Assessment Methods
- 📗 General Scene Methods
  - 📕 Statistics Methods
    - 📘 HVS-based Methods
    - 📘 Transform Domain-based Methods
    - 📘 Natural Scene Statistics-based Methods
  - 📕 Machine Learning-based Methods
    - 📘 Model-based Methods
      - 📙 Traditional Machine Learning Methods
      - 📙 CNN-based Methods
      - 📙 Transformer-based Methods
    - 📘 Framework-based Methods

- 📗 Specific Scene Methods
  - 📕 Medical IQA
  - 📕 IQA for Dehazing Algorithms
  - 📕 Portrait Quality Assessment
  - 📕 Specific Distortion
    - 📙 Blue
    - 📙 JPEG compression

## 📚 Image Quality Assessment Methods

![img2](assets/time-early.jpg)

![img3](assets/time-later.jpg)

<table>
    <tr>
        <td>Metrics</td>
        <td>Paper name</td>
        <td>Citation number as of Feb.1,2025.</td>
        <td>Earliest publication time</td>
        <td>Full/Reduced/Non Reference</td>
        <td>General/Specific Distortion</td>
    </tr>
    <tr>
        <td colspan="6" align="center">HVS-Based Method</td>
    </tr>
    <tr>
        <td>signal-to-noise ratio (SNR)</td>
        <td></td>
        <td></td>
        <td></td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>peak SNR (PSNR)</td>
        <td></td>
        <td></td>
        <td></td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>mean squared error (MSE)</td>
        <td></td>
        <td></td>
        <td></td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>structural similarity (SSIM)</td>
        <td>Image quality assessment: From error visibility to structural similarity</td>
        <td>58352</td>
        <td>2004.04</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>multi-scale SSIM (MS-SSIM)</td>
        <td>Multiscale structural similarity for image quality assessment</td>
        <td>8043</td>
        <td>2004.05</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>universal image quality index (UQI)</td>
        <td>A universal image quality index</td>
        <td>7419</td>
        <td>2002.03</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>feature similarity index (FSIM)</td>
        <td>FSIM: A feature similarity index for image quality assessment</td>
        <td>5512</td>
        <td>2011.01</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>Visual information fidelity (VIF)</td>
        <td>Image information and visual quality</td>
        <td>4861</td>
        <td>2006.02</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>most apparent distortion (MAD)</td>
        <td>Most apparent distortion: Full-reference image quality assessment and the role of strategy</td>
        <td>2250</td>
        <td>2010.01</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>Gradient magnitude similarity deviation (GMSD)</td>
        <td>Gradient magnitude similarity deviation: A highly efficient perceptual image quality index</td>
        <td>1716</td>
        <td>2013.12</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>Visual SNR (VSNR)</td>
        <td>VSNR: A wavelet-based visual signal-to-noise ratio for natural images</td>
        <td>1578</td>
        <td>2007.08</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>information content weighted SSIM measure (IW-SSIM)</td>
        <td>Information content weighting for perceptual image quality assessment</td>
        <td>1533</td>
        <td>2010.11</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>9</td>
        <td>Why is image quality assessment so difficult?</td>
        <td>1319</td>
        <td>2002.05</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>visual saliency-induced index(VSI)</td>
        <td>VSI: A visual saliency-induced index for perceptual image quality assessment</td>
        <td>1082</td>
        <td>2014.08</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>GSIM</td>
        <td>Image quality assessment based on gradient similarity</td>
        <td>872</td>
        <td>2011.11</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>complex wavelets-SSIM (CW-SSIM)</td>
        <td>Translation insensitive image similarity in complex wavelet domain</td>
        <td>455</td>
        <td>2005.05</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>HVS-based peak SNR (PSNR-HVS)</td>
        <td>A new full-reference quality metrics based on HVS</td>
        <td>433</td>
        <td>2006.01</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>RR-SSIM</td>
        <td>Reduced-reference image quality assessment by structural similarity estimation</td>
        <td>320</td>
        <td>2012.08</td>
        <td>RR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>PSIM</td>
        <td>A fast reliable image quality predictor by fusing micro- and macro-structures</td>
        <td>238</td>
        <td>2017.05</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td colspan="6" align="center">Transform Domain-Based Method</td>
    </tr>
    <tr>
        <td>BLIINDS-II</td>
        <td>Blind image quality assessment: A natural scene statistics approach in the DCT domain</td>
        <td>1912</td>
        <td>2012.03</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>87</td>
        <td>Reduced-reference image quality assessment using a wavelet-domain natural image statistic model</td>
        <td>600</td>
        <td>2005.03</td>
        <td>RR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>74</td>
        <td>An SVD-based grayscale image quality measure for local and global assessment</td>
        <td>482</td>
        <td>2006.02</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>SFF</td>
        <td>Sparse feature fidelity for perceptual image quality assessment</td>
        <td>180</td>
        <td>2013.06</td>
        <td>FR</td>
        <td></td>
    </tr>
    <tr>
        <td>80</td>
        <td>Image quality assessment: a sparse learning way</td>
        <td>55</td>
        <td>2015.07</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>QASD</td>
        <td>Sparse representation-based image quality index with adaptive sub-dictionaries</td>
        <td>50</td>
        <td>2016.06</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>81</td>
        <td>From sparse coding significance to perceptual quality: a new approach for image quality assessment</td>
        <td>50</td>
        <td>2017.11</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td colspan="6" align="center">NSS-Based Method</td>
    </tr>
    <tr>
        <td>160</td>
        <td>A statistical evaluation of recent full reference image quality assessment algorithms</td>
        <td>3526</td>
        <td>2006.10</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>IFC</td>
        <td>An information fidelity criterion for image quality assessment using natural scene statistics</td>
        <td>1721</td>
        <td>2005.11</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>Tone-mapped images quality index (TMQI)</td>
        <td>Objective quality assessment of tone-mapped images</td>
        <td>720</td>
        <td>2012.10</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>36</td>
        <td>Blind image quality assessment through anisotropy</td>
        <td>397</td>
        <td>2007.09</td>
        <td></td>
        <td>G</td>
    </tr>
    <tr>
        <td>Dynamic range independent quality measure (DRIM)</td>
        <td>Dynamic range independent image quality assessment</td>
        <td>371</td>
        <td>2008.08</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td colspan="6" align="center">Traditional Machine Learning Method</td>
    </tr>
    <tr>
        <td>The blind/referenceless image spatial quality evaluator (BRISQUE)</td>
        <td>No-reference image quality assessment in the spatial domain</td>
        <td>5733</td>
        <td>2012.08</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>distortion identification-based image verity and integrity evaluation(DIIVINE)</td>
        <td>Blind image quality assessment: From natural scene statistics to perceptual quality</td>
        <td>2003</td>
        <td>2011.01</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <!-- <tr>
        <td>Blind Image Integrity Notator using DCT Statistics（BLIINDS-II，和transform domain-based method冲突）</td>
        <td>Blind image quality assessment: A natural scene statistics approach in the DCT domain</td>
        <td>1912</td>
        <td>2012.03</td>
        <td>NR</td>
        <td>G</td>
    </tr> -->
    <!-- 这一项放在transform domain-based method了，所以从这里删除 -->
    <tr>
        <td>IL-NIQE</td>
        <td>A feature-enriched completely blind image quality evaluator</td>
        <td>1214</td>
        <td>2015.04</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>130</td>
        <td>No-reference image quality assessment using modified extreme learning machine classifier</td>
        <td>292</td>
        <td>2009.03</td>
        <td>NR</td>
        <td>G(具体有五种)</td>
    </tr>
    <tr>
        <td>multi-method fusion (MMF)</td>
        <td>Image quality assessment using multi-method fusion</td>
        <td>216</td>
        <td>2012.12</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>73</td>
        <td>Objective image quality assessment based on support vector regression</td>
        <td>200</td>
        <td>2010.01</td>
        <td>能够预测其内容和失真类型未出现在训练集中的图像的感知质量</td>
        <td></td>
    </tr>
    <tr>
        <td>SVDR</td>
        <td>SVD-based quality metric for image and video using machine learning</td>
        <td>184</td>
        <td>2011.09</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>93</td>
        <td>Blind Image Quality Assessment Based on Multichannel Feature Fusion and Label Transfer</td>
        <td>176</td>
        <td>2015.03</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>ParaBoost</td>
        <td>A paraboost method to image quality assessment</td>
        <td>86</td>
        <td>2015.12</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td colspan="6" align="center">CNN-Based Method</td>
    </tr>
    <tr>
        <td>163</td>
        <td>The Unreasonable Effectiveness of Deep Features as a Perceptual Metric</td>
        <td>12353</td>
        <td>2018.01</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>IQA-CNN</td>
        <td>Convolutional neural networks for no-reference image quality assessment</td>
        <td>1406</td>
        <td>2014.09</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>32</td>
        <td>Deep neural networks for no-reference and full-reference image quality assessment</td>
        <td>1229</td>
        <td>2017.10</td>
        <td>FR+NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>DISTS</td>
        <td>Image Quality Assessment: Unifying Structure and Texture Similarity</td>
        <td>847</td>
        <td>2020.12</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>BIQA by a Self-Adaptive Hyper Network</td>
        <td>Blindly Assess Image Quality in the Wild Guided by a Self-Adaptive Hyper Network</td>
        <td>667</td>
        <td>2020.06</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>MEON</td>
        <td>End-to-end blind image quality assessment using deep neural networks</td>
        <td>593</td>
        <td>2017.11</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>RankIQA</td>
        <td>RankIQA: Learning from rankings for no-reference image quality assessment</td>
        <td>556</td>
        <td>2017.07</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>BIECON</td>
        <td>Fully deep blind image quality predictor</td>
        <td>487</td>
        <td>2016.12</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>101</td>
        <td>Blind image quality assessment via deep learning</td>
        <td>433</td>
        <td>2014.08</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>DeepBIQ</td>
        <td>On the use of deep learning for blind image quality assessment</td>
        <td>396</td>
        <td>2016.02</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>deep image quality assessment (DeepQA)</td>
        <td>Deep learning of human visual sensitivity in image quality assessment framework</td>
        <td>304</td>
        <td>2017.10</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>DeepSim</td>
        <td>DeepSim: deep similarity for image quality assessment</td>
        <td>190</td>
        <td>2017.09</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>95</td>
        <td>Blind image quality assessment using semi-supervised rectifier networks</td>
        <td>126</td>
        <td>2014.09</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>Re-IQA</td>
        <td>Re-IQA: Unsupervised Learning for Image Quality Assessment in the Wild</td>
        <td>84</td>
        <td>2023.04</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>Multi-Pooled Inception Features for NR IQA</td>
        <td>Multi-Pooled Inception Features for No-Reference Image Quality Assessment</td>
        <td>44</td>
        <td>2020.02</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>IQMA Network</td>
        <td>IQMA Network: Image Quality Multi-Scale Assessment Network</td>
        <td>27</td>
        <td>2021.06</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td colspan="6" align="center">Transformer-Based Method</td>
    </tr>
    <tr>
        <td>MUSIQ</td>
        <td>MUSIQ: Multi-Scale Image Quality Transformer</td>
        <td>601</td>
        <td>2021.08</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>ViT with relative ranking and self-consistency</td>
        <td>No-reference image quality assessment via transformers, relative ranking,and self-consistency</td>
        <td>307</td>
        <td>2021.08</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>Maniqa</td>
        <td>Maniqa: Muli-dimension attention network for no-reference image quality assessment</td>
        <td>301</td>
        <td>2022.04</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>TRIQ</td>
        <td>Transformer for Image Quality Assessment</td>
        <td>230</td>
        <td>2020.12</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td> IQT</td>
        <td>Perceptual Image Quality Assessment With Transformers</td>
        <td>167</td>
        <td>2021.04</td>
        <td>FR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>NTIRE 2021 Challenge on Perceptual IQA</td>
        <td>NTIRE 2021 Challenge on Perceptual Image Quality Assessment</td>
        <td>114</td>
        <td>2021.05</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>NTIRE 2022 Challenge on Perceptual IQA</td>
        <td>NTIRE 2022 Challenge on Perceptual Image Quality Assessment</td>
        <td>113</td>
        <td>2022.06</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td colspan="6" align="center">Framework-Based Method</td>
    </tr>
    <tr>
        <td>QAC</td>
        <td>Learning without human scores for blind image quality assessment</td>
        <td>470</td>
        <td>2013.06</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>MetalQA</td>
        <td>MetalQA: Deep Meta-Learning for No-Reference Image Quality Assessment</td>
        <td>405</td>
        <td>2020.04</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>112</td>
        <td>Deep CNN-based blind image quality predictor</td>
        <td>315</td>
        <td>2018.06</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>UNIQUE</td>
        <td>Uncertainty-Aware Blind Image Quality Assessment in the Laboratory and Wild</td>
        <td>286</td>
        <td>2021.03</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>Hallucinated-IQA</td>
        <td>Hallucinated-IQA: No-reference image quality assessment via adversarial learning</td>
        <td>273</td>
        <td>2018.04</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>CONTRIQUE</td>
        <td>Image quality assessment using contrastive learning</td>
        <td>206</td>
        <td>2022.06</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>DeepFL-IQA</td>
        <td>DeepFL-IQA: Weak Supervision for Deep IQA Feature Learning</td>
        <td>67</td>
        <td>2020.01</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>CVRDK-IQA</td>
        <td>Content-Variant Reference Image Quality Assessment via Knowledge Distillation</td>
        <td>34</td>
        <td>2022.02</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td>CNN-Based Medical Ultrasound IQA</td>
        <td>CNN-Based Medical Ultrasound Image Quality Assessment</td>
        <td>28</td>
        <td>2021.07</td>
        <td>NR</td>
        <td>G</td>
    </tr>
    <tr>
        <td colspan="6" align="center">Medical IQA</td>
    </tr>
    <tr>
        <td>164</td>
        <td>Quantitative assessment of structural image quality</td>
        <td>360</td>
        <td>2018.04</td>
        <td>NR</td>
        <td></td>
    </tr>
    <tr>
        <td colspan="6" align="center">IQA for Dehazing Algorithm</td>
    </tr>
    <tr>
        <td>165</td>
        <td>Quality evaluation of image dehazing methods using synthetic hazy images</td>
        <td>222</td>
        <td>2019.02</td>
        <td>FR</td>
        <td>dehazing</td>
    </tr>
    <tr>
        <td colspan="6" align="center">Portrait Quality Assessment</td>
    </tr>
    <tr>
        <td>166</td>
        <td>Deep Portrait Quality Assessment. A NTIRE 2024 Challenge Survey</td>
        <td>15</td>
        <td>2024.04</td>
        <td>NR</td>
        <td></td>
    </tr>
    <tr>
        <td colspan="6" align="center">IQA for Low Light Enhancement</td>
    </tr>
    <tr>
        <td>NLIEE</td>
        <td>A no-reference evaluation metric for low-light image enhancement</td>
        <td>55</td>
        <td>2021.06</td>
        <td>NR</td>
        <td></td>
    </tr>
    <tr>
        <td colspan="6" align="center">Specific Distortion</td>
    </tr>
    <tr>
        <td>133</td>
        <td>A no-reference objective image sharpness metric based on the notion of just noticeable blur (JNB)</td>
        <td>1004</td>
        <td>2009.04</td>
        <td>NR</td>
        <td>blur distortion</td>
    </tr>
    <tr>
        <td>BIBLE</td>
        <td>No-reference image blur assessment based on discrete orthogonal moments</td>
        <td>280</td>
        <td>2015.01</td>
        <td>NR</td>
        <td>blur distortion</td>
    </tr>
    <tr>
        <td>169</td>
        <td>A no-reference metric for evaluating the quality of motion deblurring</td>
        <td>127</td>
        <td>2013.11</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>168</td>
        <td>Full reference image quality metrics for JPEG compressed images</td>
        <td>40</td>
        <td>2015.02</td>
        <td>NR</td>
        <td>JPEG</td>
    </tr>
</table>
