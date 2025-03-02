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

<table>
    <tr>
        <td>Metrics</td>
        <td>Introduction</td>
        <td>Paper name</td>
        <td>Citation number as of Feb.1,2025.</td>
        <td>Earliest publication time</td>
        <td><(Full-R, Reduced-R or Non-R)</td>
        <td>General Distortion or Specific Distortion <br>(如果是specific distortion，<br>请指出具体的distortion种类)</td>
        <td>所使用框架<br>(如果创新点在框架上，<br>如果是统计学方法则不填)</td>
        <td>所使用模型<br>(如果创新点在模型上，<br>如果是统计学方法则不填)</td>
    </tr>
    <tr>
        <td colspan="9"  align="center">HVS-Based Method</td>
    </tr>
    <tr>
        <td>signal-to-noise ratio (SNR)</td>
        <td>未考虑human visual system</td>
        <td></td>
        <td></td>
        <td></td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>peak SNR (PSNR)</td>
        <td>未考虑human visual system</td>
        <td></td>
        <td></td>
        <td></td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>mean squared error (MSE)</td>
        <td>未考虑human visual system</td>
        <td></td>
        <td></td>
        <td></td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>structural similarity (SSIM)</td>
        <td>IQA常青树，不老战神，20年过去了，</td>
        <td>Image quality assessment: From error visibility to structural similarity</td>
        <td>58352</td>
        <td>2004.04</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>multi-scale SSIM (MS-SSIM)</td>
        <td>为了将SSIM用于不同分辨率的图像，提出了MS-SSIM</td>
        <td>Multiscale structural similarity for image quality assessment</td>
        <td>8043</td>
        <td>2004.05</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>universal image quality index(UQI)</td>
        <td>通过将任何图像失真建模为三个因素的组合：相关性损失、亮度失真和对比度失真</td>
        <td>A universal image quality index</td>
        <td>7419</td>
        <td>2002.03</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>feature similarity index (FSIM)</td>
        <td>FSIM主要依赖于相位一致性（PC）和梯度幅度（GM）这两个低级特征，通过生成局部相似性图并使用相位一致性作为加权函数，将局部质量整合成单一评分</td>
        <td>FSIM: A feature similarity index for image quality assessment</td>
        <td>5512</td>
        <td>2011.01</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>Visual information fidelity(VIF)</td>
        <td> 1.VIF algorithm models natural images in wavelet domain using GSM model.<br>2.Distortion is modeled in the wavelet domain as signal attenuation and additive noise.</td>
        <td>Image information and visual quality</td>
        <td>4861</td>
        <td>2006.02</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>most apparent distortion (MAD)</td>
        <td>MAD方法通过加权几何平均的方式结合检测基础策略、外观基础策略这两种策略的输出，最终得出图像的总体质量评分。在高失真图像中，外观基础质量的权重更大；而在近阈值失真的高质量图像中，检测基础质量的权重则更大。</td>
        <td>Most apparent distortion: Full-reference image quality assessment and the role of strategy</td>
        <td>2250</td>
        <td>2010.01</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>Gradient magnitude similarity deviation (GMSD)</td>
        <td>GMSD基于图像梯度信息，通过计算参考图像与失真图像的梯度幅值相似性来评估质量，使用标准差作为池化策略</td>
        <td>Gradient magnitude similarity deviation: A highly efficient perceptual image quality index</td>
        <td>1716</td>
        <td>2013.12</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>Visual SNR (VSNR)</td>
        <td>考虑human visual system<br>  (HVS)</td>
        <td>VSNR: A wavelet-based visual signal-to-noise ratio for natural images</td>
        <td>1578</td>
        <td>2007.08</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>information content weighted SSIM measure (IW-SSIM)</td>
        <td>IW-MSE使用了多尺度信息内容权重来计算局部均方误差，IW-PSNR则是在IW-MSE的基础上将均方误差转换为峰值信噪比</td>
        <td>Information content weighting for perceptual image quality assessment</td>
        <td>1533</td>
        <td>2010.11</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>9</td>
        <td>首次提出这样一个观点，促进了SSIM的出现：<br>The main function of the human eyes is to extract structural information from the viewing field, and the human visual system is highly adapted for this purpose</td>
        <td>Why is image quality assessment so difficult?</td>
        <td>1319</td>
        <td>2002.05</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>visual saliency-induced index(VSI)</td>
        <td>VSI结合视觉显著性、梯度模和色度信息，利用视觉显著性作为局部质量特征和加权函数反映图像中不同区域的重要性</td>
        <td>VSI: A visual saliency-induced index for perceptual image quality assessment</td>
        <td>1082</td>
        <td>2014.08</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>GSIM</td>
        <td>基于SSIM, 提出的基于梯度相似性的图像质量评估方法，充分考虑了图像的梯度特征，尤其是边缘、纹理和细节部分</td>
        <td>Image quality assessment based on gradient similarity</td>
        <td>872</td>
        <td>2011.11</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>complex wavelets-SSIM (CW-SSIM)</td>
        <td>结构相似性虽然能大致符合人类的视觉系统的感受，但若图片遇到几何上的转换，例如平移、旋转与缩放时，结构相似性会无法正确描述两张图片的相似程度</td>
        <td>Translation insensitive image similarity in complex wavelet domain</td>
        <td>455</td>
        <td>2005.05</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>HVS-based peak SNR (PSNR-HVS)</td>
        <td>考虑human visual system</td>
        <td>A new full-reference quality metrics based on HVS</td>
        <td>433</td>
        <td>2006.01</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>RR-SSIM</td>
        <td>为了在评估图像质量的过程中考虑psychophysical visual masking effect，使用DNT（Divisive Normalization Transform，除法归一化变换）提取图像信息，并用于估计SSIM、评价图像质量。<br>DNT:DNT 在多尺度和多方向的小波变换基础上进行的，能够提取图像的局部结构信息，同时考虑到相邻像素或系数之间的相互影响,通过将每个系数除以一个基于其邻域系数的局部能量度量，从而实现归一化 </td>
        <td>Reduced-reference image quality assessment by structural similarity estimation</td>
        <td>320</td>
        <td>2012.08</td>
        <td>RR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>PSIM</td>
        <td>基于SSIM, 通过融合图像的微观结构和宏观结构信息，提供了一种既精确又高效的图像质量评估框架</td>
        <td>A fast reliable image quality predictor by fusing micro- and macro-structures</td>
        <td>238</td>
        <td>2017.05</td>
        <td>FR</td>
        <td>G</td>
        <td>PSIM</td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td colspan="9" align="center">Transform Domain-Based Method</td>
    </tr>
    <tr>
        <td>Blind Image Integrity Notator using DCT Statistics（BLIINDS-II）</td>
        <td>natural scene statistics (NSS)-based NR metrics</td>
        <td>Blind image quality assessment: A natural scene statistics approach in the DCT domain</td>
        <td>1912</td>
        <td>2012.03</td>
        <td>NR</td>
        <td>G</td>
        <td>NSS+DCT</td>
        <td></td>
    </tr>
    <tr>
        <td>87</td>
        <td>使用wavelet transform，利用wavelet coefficients随着图像失真发生的变化进行评估</td>
        <td>Reduced-reference image quality assessment using a wavelet-domain natural image statistic model</td>
        <td>600</td>
        <td>2005.03</td>
        <td>RR</td>
        <td>G</td>
        <td></td>
        <td>小波变换</td>
    </tr>
    <tr>
        <td>74</td>
        <td>另一种基于SVD的度量，作者首先计算参考图像块和失真图像块的奇异值之间的距离，然后计算每个块的全局值以表示最终质量。</td>
        <td>An SVD-based grayscale image quality measure for local and global assessment</td>
        <td>482</td>
        <td>2006.02</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>SFF</td>
        <td>稀疏特征保真度（SFF）度量;<br>补充：这篇paper使用ICA来模仿皮层简单细胞的视觉系统，很会讲故事啊。</td>
        <td>Sparse feature fidelity for perceptual image quality assessment</td>
        <td>180</td>
        <td>2013.06</td>
        <td>FR</td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>80</td>
        <td>在局部图像块中使用了稀疏表示，并计算了参考和失真块的稀疏表示之间的差异，作为质量图。采用核岭回归（KRR）将局部质量融合到最终的质量分数中。</td>
        <td>Image quality assessment: a sparse learning way</td>
        <td>55</td>
        <td>2015.07</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>QASD</td>
        <td>一种基于稀疏表示的自适应子字典（QASD）图像质量指数</td>
        <td>Sparse representation-based image quality index with adaptive sub-dictionaries</td>
        <td>50</td>
        <td>2016.06</td>
        <td>FR</td>
        <td>G</td>
        <td>QASD</td>
        <td></td>
    </tr>
    <tr>
        <td>81</td>
        <td>首先为稀疏编码部署了傅立叶基，然后对稀疏系数的幅度进行了排序，最后评估了参考图像和失真图像的排序系数之间的对应性。</td>
        <td>From sparse coding significance to perceptual quality: a new approach for image quality assessment</td>
        <td>50</td>
        <td>2017.11</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td colspan="9" align="center">NSS-Based Method</td>
    </tr>
    <tr>
        <td>160</td>
        <td>提出一个大规模主观质量评估数据集，对 10 种主流全参考图像质量评估算法进行系统对比，发现其效果不佳，有很大进步空间</td>
        <td>A statistical evaluation of recent full reference image quality assessment algorithms</td>
        <td>3526</td>
        <td>2006.10</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>IFC</td>
        <td></td>
        <td>An information fidelity criterion for image quality assessment using natural scene statistics</td>
        <td>1721</td>
        <td>2005.11</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td>NSS</td>
    </tr>
    <tr>
        <td>Tone-mapped images quality index—TMQI（调整后的色调映射图像质量指数）</td>
        <td>是一种用于评估色调映射图像质量的全参考图像质量评估（FR-IQA）方法。它结合了多尺度结构保真度测量和统计自然度测量，以客观地评估由色调映射算子（TMO）生成的低动态范围（LDR）图像的质量</td>
        <td>Objective quality assessment of tone-mapped images</td>
        <td>720</td>
        <td>2012.10</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>36</td>
        <td>通过图像的anisotropy评估其质量。</td>
        <td>Blind image quality assessment through anisotropy</td>
        <td>397</td>
        <td>2007.09</td>
        <td></td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>Dynamic range independent quality measure—DRIM（动态范围独立度量）</td>
        <td>test image 和 reference image可能scale不同，该方法在评估质量时可以无视尺度scale</td>
        <td>Dynamic range independent image quality assessment</td>
        <td>371</td>
        <td>2008.08</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td colspan="9" align="center">Traditional Machine Learning  Method</td>
    </tr>
    <tr>
        <td>The blind/referenceless image spatial quality evaluator (BRISQUE)</td>
        <td>natural scene statistics (NSS)-based NR metrics;</td>
        <td>No-reference image quality assessment in the spatial domain</td>
        <td>5733</td>
        <td>2012.08</td>
        <td>NR</td>
        <td>G</td>
        <td>Natural Scene Statistics（NSS）</td>
        <td></td>
    </tr>
    <tr>
        <td>distortion identification-based image verity and integrity evaluation(DIIVINE)</td>
        <td>natural scene statistics (NSS)-based NR metrics</td>
        <td>Blind image quality assessment: From natural scene statistics to perceptual quality</td>
        <td>2003</td>
        <td>2011.01</td>
        <td>NR</td>
        <td>G</td>
        <td>Natural Scene Statistics（NSS）</td>
        <td></td>
    </tr>
    <tr>
        <td>Blind Image Integrity Notator using DCT Statistics（BLIINDS-II，和transform domain-based method冲突）</td>
        <td>natural scene statistics (NSS)-based NR metrics</td>
        <td>Blind image quality assessment: A natural scene statistics approach in the DCT domain</td>
        <td>1912</td>
        <td>2012.03</td>
        <td>NR</td>
        <td>G</td>
        <td>NSS+DCT</td>
        <td></td>
    </tr>
    <tr>
        <td>IL-NIQE</td>
        <td>使用natural scene statistics (NSS)-based methods抽取reliable features；<br>从互联网上筛选90长高质量图片，以此训练MVG模型，通过计算图片与原始MVG模型的距离给图片打分。<br>补充：<br>使用从图像中提取的NSS特征学习一个multivariate Gaussian (MVG) model，用于评估图像质量</td>
        <td>A feature-enriched completely blind image quality evaluator</td>
        <td>1214</td>
        <td>2015.04</td>
        <td>NR</td>
        <td>G</td>
        <td>MVG</td>
        <td></td>
    </tr>
    <tr>
        <td>130</td>
        <td>NR类型，HVS features such as edge ampli-tude,edge length,background activity and back groundluminance   are used.These features along with MOS of images are fed to extreme machine learning(ELM)[27]algorithm to obtain a func-tional relationship.<br>补充：<br>提取空间和频谱熵特征（Spatial and Spectral Entropy Features），并使用单隐藏层前馈神经网络极限学习机（Extreme Learning Machine, ELM）确定失真类型，并估计失真程度。</td>
        <td>No-reference image quality assessment using modified extreme learning machine classifier</td>
        <td>292</td>
        <td>2009.03</td>
        <td>NR</td>
        <td>G(具体有五种)</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>multi-method fusion (MMF)</td>
        <td>不同的质量评估方法各有优劣，不妨将其全部整合起来，随后采用支持向量回归（SVR）来整合多个质量指标的得分</td>
        <td>Image quality assessment using multi-method fusion</td>
        <td>216</td>
        <td>2012.12</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td>SVR</td>
    </tr>
    <tr>
        <td>73</td>
        <td>使用了基于奇异值分解（SVD）的特征，并将支持向量回归（SVR）用作特征融合工具。</td>
        <td>Objective image quality assessment based on support vector regression</td>
        <td>200</td>
        <td>2010.01</td>
        <td>能够预测其内容和失真类型未出现在训练集中的图像的感知质量</td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>SVDR</td>
        <td>使用：<br>奇异值分解SVD<br>进行特征提取，<br>使用<br>机器学习支持向量退化SVDR<br>进行特征融合。</td>
        <td>SVD-based quality metric for image and video using machine learning</td>
        <td>184</td>
        <td>2011.09</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>93</td>
        <td>Inspired by the hierarchical and trichromatic properties of human vision, we extract both the frequency and spatial-frequency features from all three YCbCr channels to describe a natural image. Then, a KNN(k-nearest-neighbor)-based LT(Label Transfer) model is used to estimate the query image’s quality.</td>
        <td>Blind Image Quality Assessment Based on Multichannel Feature Fusion and Label Transfer</td>
        <td>176</td>
        <td>2015.03</td>
        <td>NR</td>
        <td>G</td>
        <td></td>
        <td>KNN</td>
    </tr>
    <tr>
        <td>ParaBoost</td>
        <td>Paraboost method based on SVR</td>
        <td>A paraboost method to image quality assessment</td>
        <td>86</td>
        <td>2015.12</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td colspan="9" align="center">CNN-Based  Method</td>
    </tr>
    <tr>
        <td>163</td>
        <td>提出了一个新的人类感知相似性判断数据集。<br>评估了不同架构和任务中的深度特征，并将它们与经典指标进行比较。发现在该数据集上深度特征的表现大大优于以前的所有指标。</td>
        <td>The Unreasonable Effectiveness of Deep Features as a Perceptual Metric</td>
        <td>12353</td>
        <td>2018.01</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>IQA-CNN</td>
        <td>A pioneering work.</td>
        <td>Convolutional neural networks for no-reference image quality assessment</td>
        <td>1406</td>
        <td>2014.09</td>
        <td>NR</td>
        <td>G</td>
        <td></td>
        <td>CNN</td>
    </tr>
    <tr>
        <td>32</td>
        <td>通过Siamese结构处理参考图像和失真图像，实现特征的共享和比较；<br>提出三个网络，WaDIQaM - NR，DIQaM - NR，WaDIQaM-FR</td>
        <td>Deep neural networks for no-reference and full-reference image quality assessment</td>
        <td>1229</td>
        <td>2017.10</td>
        <td>FR&amp;NR</td>
        <td>G</td>
        <td></td>
        <td>DNN</td>
    </tr>
    <tr>
        <td>DISTS</td>
        <td>大多CNN-based FR IQA方法对图像的texture similarity过于敏感，DISTS作为the first of its kind with built-in tolerance to texture resampling，基于VGG提取texture information，将structure and texture information很好地结合了起来</td>
        <td>Image Quality Assessment: Unifying Structure and Texture Similarity</td>
        <td>847</td>
        <td>2020.12</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td>VGG</td>
    </tr>
    <tr>
        <td>BIQA by a Self-Adaptive Hyper Network</td>
        <td>提出一种基于自适应超网络的图像质量评估模型，通过将 IQA 过程分为内容理解、感知规则学习和质量预测三个阶段，实现了对自然场景图像质量的有效评估。</td>
        <td>Blindly Assess Image Quality in the Wild Guided by a Self-Adaptive Hyper Network</td>
        <td>667</td>
        <td>2020.06</td>
        <td>NR</td>
        <td>G</td>
        <td>Self-Adaptive Hyper Network</td>
        <td></td>
    </tr>
    <tr>
        <td>MEON</td>
        <td>DNN methods for BIQA;<br>DNN-based BIQA using deep features and quality prediction together;<br>predicting image quality scores;<br>The image-input methods;<br>Expanding distorted images</td>
        <td>End-to-end blind image quality assessment using deep neural networks</td>
        <td>593</td>
        <td>2017.11</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>RankIQA</td>
        <td></td>
        <td>RankIQA: Learning from rankings for no-reference image quality assessment</td>
        <td>556</td>
        <td>2017.07</td>
        <td>NR</td>
        <td>G</td>
        <td></td>
        <td>CNN</td>
    </tr>
    <tr>
        <td>BIECON</td>
        <td>使用FR-IQA指标生成的局部质量图作为中间回归目标 </td>
        <td>Fully deep blind image quality predictor</td>
        <td>487</td>
        <td>2016.12</td>
        <td>NR</td>
        <td>G</td>
        <td></td>
        <td>CNN</td>
    </tr>
    <tr>
        <td>101</td>
        <td>DNN methods for BIQA;<br>DNN-based BIQA using deep features and quality prediction together;<br>predicting image quality categories<br>DNN直接根据质量给图像分等级</td>
        <td>Blind image quality assessment via deep learning</td>
        <td>433</td>
        <td>2014.08</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>DeepBIQ</td>
        <td>DNN methods for BIQA;<br>DNN-based BIQA using deep features and quality prediction together;<br>predicting image quality categories<br>DNN直接根据质量给图像分等级</td>
        <td>On the use of deep learning for blind image quality assessment</td>
        <td>396</td>
        <td>2016.02</td>
        <td>NR</td>
        <td>G</td>
        <td></td>
        <td>CNN</td>
    </tr>
    <tr>
        <td>deep image quality assessment (DeepQA)</td>
        <td></td>
        <td>Deep learning of human visual sensitivity in image quality assessment framework</td>
        <td>304</td>
        <td>2017.10</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td>DNN+HVS</td>
    </tr>
    <tr>
        <td>DeepSim</td>
        <td>一种基于深度神经网络（DNN）的深度相似性指数（DeepSim）。<br>补充：以预训练好的VGGnet为基础</td>
        <td>DeepSim: deep similarity for image quality assessment</td>
        <td>190</td>
        <td>2017.09</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td>VGG</td>
    </tr>
    <tr>
        <td>95</td>
        <td>DNN methods for BIQA;<br>SVR-based BIQA using deep features extracted by DNN;<br>Extracting from low-level features;</td>
        <td>Blind image quality assessment using semi-supervised rectifier networks</td>
        <td>126</td>
        <td>2014.09</td>
        <td>NR</td>
        <td>G</td>
        <td>Semi-supervised Learning</td>
        <td>Rectifier Neural Network</td>
    </tr>
    <tr>
        <td>Re-IQA</td>
        <td>提出一种由Content-Aware Encoder和Quality-Aware Encoder两个encoder组成的Mixture of Experts框架，其中用到了contrastive learning进行训练。</td>
        <td>Re-IQA: Unsupervised Learning for Image Quality Assessment in the Wild</td>
        <td>84</td>
        <td>2023.04</td>
        <td>NR</td>
        <td>G</td>
        <td>Mixture of Experts, contrastive learning</td>
        <td></td>
    </tr>
    <tr>
        <td>Multi-Pooled Inception Features for NR IQA</td>
        <td>使用Inception模块的特点（包含多种卷积核大小的滤波器），并行处理不同scale的视觉信息。</td>
        <td>Multi-Pooled Inception Features for No-Reference Image Quality Assessment</td>
        <td>44</td>
        <td>2020.02</td>
        <td>NR</td>
        <td>G</td>
        <td></td>
        <td>Inception</td>
    </tr>
    <tr>
        <td>IQMA Network(21 NTIRE public leaderboard冠军)</td>
        <td>为了评价GAN 生成的图像中通常具有的看似真实却虚假的细节和纹理，提出双分支多尺度的FR-IQA方法。</td>
        <td>IQMA Network: Image Quality Multi-Scale Assessment Network</td>
        <td>27</td>
        <td>2021.06</td>
        <td>FR</td>
        <td>G</td>
        <td>multi-scale</td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td colspan="9" align="center">Transformer-Based  Method</td>
    </tr>
    <tr>
        <td>MUSIQ</td>
        <td>一个通过Multi-scale Patch Embedding方法处理多种size的图片，而不用对其进行裁剪、强行调整大小，从而对分辨率和纵横比敏感的场景下的IQA有奇效的MUSIQ方法。</td>
        <td>MUSIQ: Multi-Scale Image Quality Transformer</td>
        <td>601</td>
        <td>2021.08</td>
        <td>NR</td>
        <td>G</td>
        <td>Transformer</td>
        <td></td>
    </tr>
    <tr>
        <td>ViT with relative ranking and self-consistency</td>
        <td>通过修改loss function的方式，解决了现有模型无法利用relative ranking相对排名信息的缺点和无法处理等变变换的风险。</td>
        <td>No-reference image quality assessment via transformers, relative ranking,and self-consistency</td>
        <td>307</td>
        <td>2021.08</td>
        <td>NR</td>
        <td>G</td>
        <td></td>
        <td> transformers, relative ranking, and self-consistency</td>
    </tr>
    <tr>
        <td>Maniqa</td>
        <td>一种新的由ViT, swin-transformer揉合而成的、可以考虑不同通道间信息的NR-IQA方法: MANIQA</td>
        <td>Maniqa: Muli-dimension attention network for no-reference image quality assessment</td>
        <td>301</td>
        <td>2022.04</td>
        <td>NR</td>
        <td>G</td>
        <td>swin transformer, ViT</td>
        <td></td>
    </tr>
    <tr>
        <td>TRIQ</td>
        <td>在使用CNN进行图像质量评估时，往往需要固定输入，无法处理多种分辨率的图像，因此要对初始图像进行缩放，从而使得原始信息丢失，而transformer可以处理不同分辨率的图像，因此用于评估图像质量非常有效。</td>
        <td>Transformer for Image Quality Assessment</td>
        <td>230</td>
        <td>2020.12</td>
        <td>NR</td>
        <td>G</td>
        <td>ViT</td>
        <td></td>
    </tr>
    <tr>
        <td> IQT</td>
        <td>使用Siamese架构提取reference image和distorted image的特征，并使用ViT评估质量</td>
        <td>Perceptual Image Quality Assessment With Transformers</td>
        <td>167</td>
        <td>2021.04</td>
        <td>FR</td>
        <td>G</td>
        <td>Vision transformer(ViT)+Siamese</td>
        <td></td>
    </tr>
    <tr>
        <td>NTIRE 2021 Challenge on Perceptual IQA</td>
        <td></td>
        <td>NTIRE 2021 Challenge on Perceptual Image Quality Assessment</td>
        <td>114</td>
        <td>2021.05</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>NTIRE 2022 Challenge on Perceptual IQA</td>
        <td></td>
        <td>NTIRE 2022 Challenge on Perceptual Image Quality Assessment</td>
        <td>113</td>
        <td>2022.06</td>
        <td></td>
        <td></td>
        <td>ViT+CNN</td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td colspan="9" align="center">Framework-Based Method</td>
    </tr>
    <tr>
        <td>QAC</td>
        <td>不需要人类的打分即可完成IQA</td>
        <td>Learning without human scores for blind image quality assessment</td>
        <td>470</td>
        <td>2013.06</td>
        <td>NR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>MetalQA</td>
        <td>一种使用元学习解决NR-IQA任务泛化问题的方法</td>
        <td>MetalQA: Deep Meta-Learning for No-Reference Image Quality Assessment</td>
        <td>405</td>
        <td>2020.04</td>
        <td>NR</td>
        <td>G</td>
        <td>Meta-Learning</td>
        <td></td>
    </tr>
    <tr>
        <td>112</td>
        <td>DNN methods for BIQA;<br>DNN-based BIQA using deep features and quality prediction together;<br>predicting image quality scores;<br>The patch-input methods;<br>FR as patch label;<br>这个工作很贼，使用的patch的label是error map</td>
        <td>Deep CNN-based blind image quality predictor</td>
        <td>315</td>
        <td>2018.06</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>UNIQUE</td>
        <td>UNIQUE是一个具有cross-distortion-scenario generalization能力的BIQA模型，并且提出a method of training it on multiple IQA databases simultaneously，从而可以在训练一种distortion上的模型时，使用其他distortion类型的数据。</td>
        <td>Uncertainty-Aware Blind Image Quality Assessment in the Laboratory and Wild</td>
        <td>286</td>
        <td>2021.03</td>
        <td>NR</td>
        <td>G</td>
        <td>UNIQUE</td>
        <td></td>
    </tr>
    <tr>
        <td>Hallucinated-IQA</td>
        <td>利用质量感知生成网络生成高分辨率的虚幻图像，并结合对比图像与虚幻图像之间的差异图来训练质量回归网络</td>
        <td>Hallucinated-IQA: No-reference image quality assessment via adversarial learning</td>
        <td>273</td>
        <td>2018.04</td>
        <td>NR</td>
        <td>G</td>
        <td>adversarial learning</td>
        <td>CNN</td>
    </tr>
    <tr>
        <td>CONTRIQUE</td>
        <td>开发基于CNN的IQA模型的一个障碍是缺乏足够大的标记IQA数据集。所以大多数基于CNN的IQA模型都利用了迁移学习，即CNN在像ImageNet这样的大型数据集上进行预训练，然后对具有主观质量判断的图像进行端到端精细调整。<br>尽管经过微调的模型在合成失真和真实失真方面都取得了令人印象深刻的性能，但微调需要仔细选择超参数，这些超参数可能随不同的IQA数据库而变化。此外，过度的微调会使模型对训练数据过拟合，限制了模型的泛化能力。<br>该文引入了一个基于对比学习的IQA训练框架，旨在使用无标记数据集获得高效的图像质量表示。<br>该文使用畸变类型和程度的预测作为辅助任务，从包含合成和真实混合失真的未标记图像数据集学习特征。然后训练一个深度卷积神经网络(CNN)使用一个contrastive pairwise来解决辅助问题。<br>然后将提出的训练框架和产生的深层IQA模型作为对比图像质量评估器(CONTRIQUE)。在评估期间，CNN权重被冻结，线性回归器将学习的表示映射到NR设置中的质量分数。通过大量的实验表明，与最先进的NR图像质量模型相比，CONTRIQUE获得了具有竞争力的性能，即使没有任何额外的CNN骨干微调。<br>学习后的表征具有高度的鲁棒性，并且在受合成或真实扭曲影响的图像中具有很好的泛化能力。结果表明，不需要大量标注主观图像质量数据集，就可以获得具有感知相关性的强大质量表征</td>
        <td>Image quality assessment using contrastive learning</td>
        <td>206</td>
        <td>2022.06</td>
        <td>NR</td>
        <td>G</td>
        <td>contrastive learning, self-supervised learning</td>
        <td></td>
    </tr>
    <tr>
        <td>DeepFL-IQA</td>
        <td>DeepFL-IQA提出一种基于weak supervision learning的方法，在训练过程中使用大量的客观IQA指标打出的分数作为参考，再使用主观质量分数作为参考进行微调，以获得预测出符合HVS分数的能力。</td>
        <td>DeepFL-IQA: Weak Supervision for Deep IQA Feature Learning</td>
        <td>67</td>
        <td>2020.01</td>
        <td>NR</td>
        <td>G</td>
        <td>Weak Supervision Learning</td>
        <td>CNN</td>
    </tr>
    <tr>
        <td>CVRDK-IQA</td>
        <td>比起NR方法，FR方法效果往往更好，本文利用知识蒸馏，能够把FR学到的东西教给NR：将 FR-teacher 中的知识传递给 NAR-student，从而使 NAR-student 能够在没有pixel level对齐的参考图像的情况下进行图像质量评估。两组模型结构完全相同。<br>虽然我没有参考图像，但我知道参考图像应该是什么样的</td>
        <td>Content-Variant Reference Image Quality Assessment via Knowledge Distillation</td>
        <td>34</td>
        <td>2022.02</td>
        <td>NR</td>
        <td>G</td>
        <td>Knowledge Distillation</td>
        <td></td>
    </tr>
    <tr>
        <td>CNN-Based Medical Ultrasound IQA</td>
        <td>鉴于超声图像样本不丰富，引入迁移学习策略。利用光学图像数据集对CNN模型进行预训练，然后再用超声图像进行微调，有效解决了超声图像数据有限导致的过拟合问题。</td>
        <td>CNN-Based Medical Ultrasound Image Quality Assessment</td>
        <td>28</td>
        <td>2021.07</td>
        <td>NR</td>
        <td>G</td>
        <td>transfer learning</td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td colspan="9" align="center">Medical IQA</td>
    </tr>
    <tr>
        <td>164</td>
        <td>在脑成像研究中，数据质量是一个重要的混杂因素，尤其是在脑发育研究中，年龄与扫描仪内的运动和数据质量系统相关。该论文研究评估了多种定量图像质量指标，包括Preprocessed Connectomes Project&#39;s Quality Assurance Protocol (QAP)提供的指标和FreeSurfer提供的Euler number。<br>在多种质量指标中，Euler number表现最好。原因在于某些指标（如信噪比（SNR）和对比噪声比（CNR））评估的是图像的全局特性，而Euler数评估的是局部的拓扑结构。局部的运动伪影或重建错误可能对全局指标的影响较小，但对Euler数的影响较大。例如，一个局部的运动伪影可能导致皮层表面出现孔洞或断裂，从而显著影响Euler数，但对SNR或CNR的影响可能不明显。<br>这表明在实际应用中，选择合适的质量评估指标需要根据具体的研究需求和数据特点来决定。</td>
        <td>Quantitative assessment of structural image quality</td>
        <td>360</td>
        <td>2018.04</td>
        <td>NR</td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td colspan="9" align="center">IQA for Dehazing Algorithm</td>
    </tr>
    <tr>
        <td>165</td>
        <td>图像去雾算法（Dehazing Algorithms，简称DHAs）是一类用于改善在雾霾等恶劣天气条件下拍摄的图像质量的算法。这些算法的目标是去除图像中的雾气，恢复图像的清晰度、对比度和色彩，从而提高图像的视觉质量和可用性。<br>现有的FR IQA方法不适用于DHA的评估，主要是因为去雾过程不仅仅是图像恢复，还涉及到对比度增强、色彩调整和结构恢复等多个方面。这些特性使得传统的FR IQA方法在评估去雾效果时存在局限性。<br>本文提出的去雾算法评估方法通过综合考虑图像结构恢复Image Structure Recovering、色彩再现Color Rendition和低对比度区域的过度增强Over-Enhancement of Low-Contrast Areas，能够更全面地评估去雾算法的效果。该方法不仅适应了去雾过程中的对比度增强和色彩调整，还通过针对航拍图像的改进，提高了评估方法的适用性和准确性。</td>
        <td>Quality evaluation of image dehazing methods using synthetic hazy images</td>
        <td>222</td>
        <td>2019.02</td>
        <td>FR</td>
        <td>dehazing</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td colspan="9" align="center">Portrait Quality Assessment</td>
    </tr>
    <tr>
        <td>166</td>
        <td>随着智能手机的普及，肖像摄影变得普遍，但实现专业质量的图像仍然是一个挑战。<br>在肖像中，面部区域通常是视觉焦点，其质量对整体肖像质量的影响远大于其他区域。传统IQA方法通常对整幅图像进行全局评估，难以捕捉到面部区域的特殊重要性。同时，肖像质量不仅取决于面部区域的质量，还与背景、构图等全局因素密切相关。传统IQA方法往往难以同时兼顾局部和全局的质量评估。因此需要提出开发专门的肖像质量评估方法。<br>NTIRE 2024 Challenge——Deep Portrait Quality Assessment中的参赛队伍纷纷提出了自己的方法，例如PQE提出了一种两分支肖像质量评估模型，分别对全图和面部组件进行建模，并使用LIQE提取场景和质量特征；SAR提出了一种场景自适应全局上下文和局部面部感知网络，通过面部检测器精确定位面部区域，并使用Vision Transformer对局部面部区域和全局图像进行建模。</td>
        <td>Deep Portrait Quality Assessment. A NTIRE 2024 Challenge Survey</td>
        <td>15</td>
        <td>2024.04</td>
        <td>NR</td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td colspan="9" align="center">IQA for Low Light Enhancement</td>
    </tr>
    <tr>
        <td>NLIEE</td>
        <td>低光照图像增强算法（Low-Light Image Enhancement Algorithms，LIEAs）是一类专门用于改善在低光照条件下拍摄的图像质量的算法。该算法需要提高图像的整体亮度，调整图像的对比度，减少图像中的噪声，调整图像的色彩。<br>为了准确评估低光照图像增强算法的效果，需要一种能够综合考虑多种失真类型和复杂性的评估方法。这种评估方法需要能够从亮度增强、色彩对比、噪声水平和结构完整性等多个维度评估图像质量。<br>NLIEE是首个专门为低光照图像增强质量评估设计的无参考评估指标，其从四个关键方面提取特征，全面评估低光照图像增强后的质量：光照增强，色彩对比，噪声测量，结构评估。与通用的评估方法相比，具有更高的准确性和相关性。</td>
        <td>A no-reference evaluation metric for low-light image enhancement</td>
        <td>55</td>
        <td>2021.06</td>
        <td>NR</td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td colspan="9" align="center">Specific Distortion</td>
    </tr>
    <tr>
        <td>133</td>
        <td>NR类型，仅将锐度作为一个指标，<br>JNB comes from just noticeable difference(JND) and is the minimum difference inintensity value relative to background that is noticeable.JNB is the minimum perceivable blur around an edge givenahighercontrastthanaJND</td>
        <td>A no-reference objective image sharpness metric based on the notion of just noticeable blur (JNB)</td>
        <td>1004</td>
        <td>2009.04</td>
        <td>NR</td>
        <td>blur distortion</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>BIBLE</td>
        <td>特定于某一类型(distortion specific approach)的IQA方法，需要一些先验知识，遇到未知来源的distotion就无能为力。</td>
        <td>No-reference image blur assessment based on discrete orthogonal moments</td>
        <td>280</td>
        <td>2015.01</td>
        <td>NR</td>
        <td>blur distortion</td>
        <td>离散Tchebichef矩</td>
        <td></td>
    </tr>
    <tr>
        <td>169</td>
        <td>图像去模糊（Image Deblurring）是计算机视觉和图像处理领域的一个重要任务，旨在从模糊图像中恢复出清晰的图像内容。模糊可能由多种因素引起，如相机抖动、物体运动、焦点不准确或大气湍流等。图像去模糊的目标是通过算法消除这些模糊，恢复出原始的清晰图像。<br>去模糊算法的目标是恢复出清晰的图像，但实际中很难完全恢复出理想的清晰图像。去模糊算法可能引入各种伪影，这些伪影对图像的感知质量有显著影响。例如，振铃伪影（在边缘附近出现的波纹状结构）是去模糊算法中最常见的伪影之一，它对人类视觉系统的干扰非常大。<br>不同的去模糊算法可能产生不同类型的伪影，这些伪影的特征和影响方式各不相同。因此，需要一种能够专门针对这些伪影进行评估的方法。<br>该算法设计了一系列专门针对去模糊伪影的特征，包括：<br>提出了一种新的无参考方法（PyrRing）来检测大规模振铃伪影；使用多种方法来评估去模糊结果中的噪声水平；使用多种锐度度量方法来评估去模糊结果的清晰度。这些特征能够全面评估去模糊结果的质量，而不仅仅是单一类型的伪影。</td>
        <td>A no-reference metric for evaluating the quality of motion deblurring</td>
        <td>127</td>
        <td>2013.11</td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>168</td>
        <td>在JPEG压缩过程中，块效应（Blocking Effect）和模糊效应（Blurring Effect）是需要重点解决的问题，本方法针对这两种图像退化提出了评估JPEG压缩图像质量的方法，有效捕捉了这些distortion，起到了比通用IQA方法更好的效果。</td>
        <td>Full reference image quality metrics for JPEG compressed images</td>
        <td>40</td>
        <td>2015.02</td>
        <td>NR</td>
        <td>JPEG</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
        <td></td>
    </tr>
    <tr>
         <td colspan="9" align="center">以下在其它部分使用</td>
    </tr>
    <tr>
        <td> Single stimulus categorical rating(SIQA)</td>
        <td>测试图像会在屏幕上显示一段时间，之后图像消失，观察者需要根据一个抽象的五分类尺度（优秀、良好、中等、差、极差）对图像质量进行评分。</td>
        <td>Methodology for the subjective assessment of the quality of television pictures</td>
        <td>1004</td>
        <td>2002（具体月份没有找到）</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>Double stimulus categorical rating(SIQA)</td>
        <td>与单刺激分类评分方法类似，不同之处在于，这种方法会同时显示测试图像和参考图像一段时间。之后，图像消失，观察者需要根据之前提到的五分类尺度对测试图像的质量进行评分</td>
        <td>Methodology for the subjective assessment of the quality of television pictures</td>
        <td>1004</td>
        <td>2003（具体月份没有找到）</td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>157</td>
        <td>从aesthetic point of view出发，以Composition, Lighting, Focus Controlling, Color为标准评估图像。</td>
        <td>Photo and video quality evaluation: Focusing on the subject</td>
        <td>644</td>
        <td>2008.10</td>
        <td></td>
        <td>美学图像</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>Reduced - Reference Image Quality Metric for Contrast Change(RIQMC)</td>
        <td>评估对比度变化造成的图像质量变化；<br>从相似度和舒适度两个角度评价图像质量：<br>相似度由熵的差异、相位一致性组成；<br>舒适度使用四阶的统计量（均值、方差、偏度、峰度）。<br>随后将二者线性融合。</td>
        <td>The analysis of image contrast: From quality assessment to automatic enhancement</td>
        <td>405</td>
        <td>2015.01</td>
        <td>RR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>OSVP for RR IQA</td>
        <td>通过模仿皮质细胞间相互作用来提取 OSVP 特征(orientation-selectivity-based visual pattern)用于视觉信息表示。<br>先计算像素梯度方向作为其方向，根据方向相似性确定像素间相互作用类型（兴奋或抑制），然后基于此计算像素的 OSVP，最后将具有相同 OSVP 的像素组合，将图像映射为基于 OSVP 的直方图。<br>各种失真会改变图像结构和像素间空间相关性，导致 OSVP 类型变化。通过计算参考图像和失真图像基于 OSVP 直方图的相似度来衡量质量退化。<br>评价：作者显然有脑科学背景！</td>
        <td>Orientation selectivity based visual pattern for reduced-reference image quality assessment</td>
        <td>105</td>
        <td>2016.07</td>
        <td>RR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>RR IQA using SDM</td>
        <td>定义原始和失真图像的结构退化信息（structural degradation information），通过其距离的非线性组合或 SVM 积分开发基于 结构退化模型 structural degradation model 的 RR 图像质量度量。</td>
        <td>A new reduced-reference image quality assessment using structural degradation model</td>
        <td>86</td>
        <td>2013.05</td>
        <td>RR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
    <tr>
        <td>MLIQM</td>
        <td>MLIQM first classifies a distorted image into five scales using multi-support vector machine (SVM) classification according to the quality scale recommended by the ITU, and then uses an SVR to predict the final score of the distorted image<br>经典机器学习方法</td>
        <td>Machine learning to design full-reference image quality assessment algorithm</td>
        <td>67</td>
        <td></td>
        <td>FR</td>
        <td>G</td>
        <td></td>
        <td></td>
    </tr>
</table>
