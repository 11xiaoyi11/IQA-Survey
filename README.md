# A Survey on IQA: Insights, Analysis, and Future Outlook

![img1](assets/Metric_Struct.jpg)

## 🔍 Introduction

Image Quality Assessment (IQA) is a critical component of image-related technologies and plays a pivotal role in the advancement of image processing and computer vision. In recent years, the proliferation of novel training frameworks and machine learning models has given rise to a multitude of IQA methodologies. This survey conducts a comprehensive review of nearly 200 IQA-related publications, synthesizing key developments in the field and systematically categorizing existing approaches based on their underlying models, training frameworks, publication timelines, application scenarios, and academic impact. This structured analysis aims to facilitate a swift introduction for newcomers while providing seasoned researchers with a clearer perspective on the current state of the field. Moreover, we offer a critical evaluation of the advantages and limitations of various IQA methods and present our perspectives on future research directions. To complement the survey, this repository compiles both the IQA techniques discussed in the paper and other approaches that could not be included due to space constraints, thereby serving as a valuable resource to support further advancements in IQA research.<br>

图像质量评估（IQA）在图像相关的技术中起着非常重要的作用，对于图像处理和计算机视觉领域的技术发展有着深远的影响。近年来，随着新型训练框架和机器学习模型的出现，许多IQA方法涌现出来。本综述通过调研接近二百篇IQA相关论文，总结了IQA发展中值得关注的工作，并按照不同方法所用的模型、训练框架、发表时间、使用场景和影响力进行了整理，以方便初学者快速入门、资深研究者更好地了解领域发展现状。随后，我们对诸多IQA方法的优缺点进行了分析，对IQA方法的未来发展提出了自己的见解。本repository旨在列出论文中提到的、以及受篇幅限制未提到的经典IQA方法，配合论文阅读，以促进IQA技术的发展。

🚀English Paper link: [A Survey on Image Quality Assessment: Insights, Analysis, and Future Outlook](https://arxiv.org/abs/2502.08540)<br>
🚀Chinese Paper link: [在计算机视觉领域中，我们应该如何评估图像质量（万字长文）？](https://zhuanlan.zhihu.com/p/25680975953)<br>
🚀The simplified chinese version: [什么样的图像才是好的图像？近200篇文献总结图像质量检测的最新进展与挑战](https://mp.weixin.qq.com/s/b62C0hd6DkCDaUqFIgTBng)
## Update Records

- 🔥 [Mar.2,2025] The chinese version of our survey has been released on zhihu.
- 🔥 [Feb.12,2025] The first version of our survey has been released on arXiv.

## 📜 Table of Contents

- [📚 Image Quality Assessment Methods](#-Image-Quality-Assessment-Methods)
  - 📗 General Scene Methods
    - 📕 Statistics Methods
      - 📘 [HVS-based Methods](#1)
      - 📘 [Transform Domain-based Methods](#2)
      - 📘 [Natural Scene Statistics-based Methods](#3)
    - 📕 Machine Learning-based Methods
      - 📘 Model-based Methods
        - 📙 [Traditional Machine Learning Methods](#4)
        - 📙 [CNN-based Methods](#5)
        - 📙 [Transformer-based Methods](#6)
      - 📘 [Framework-based Methods](#7)

  - 📗 Specific Scene Methods
    - 📕 [Medical IQA](#8)
    - 📕 [IQA for Dehazing Algorithms](#9)
    - 📕 [Portrait Quality Assessment](#10)
    - 📕 [Specific Distortion](#12)
      - 📙 Blue
      - 📙 JPEG compression

[👨‍💻 Contributers](#-Contributers)
 - Zhengyi Shi@[11xiaoyi11](https://github.com/11xiaoyi11)
 - Chengqian Ma@[step-out](https://github.com/step-out) 
 - Weixuan Jin@[axax11344](https://github.com/axax11344) 

[💡 Citation](#-Citation)

- If you find this survey useful, please consider citing it.

[📧 Contact Us](#-Contact-Us)

## 📚 Image Quality Assessment Methods

![img2](assets/time-early.jpg)

![img3](assets/time-later.jpg)

Citation counts below were queried from **OpenAlex on October 13, 2026**.
Paper identities were matched automatically by normalized exact title and publication year;
these matches have not been individually verified. Counts link to their OpenAlex records.
** ** marks unresolved matches, not zero. Rows without a specific paper retain blank cells.
OpenAlex counts use a different database coverage and version grouping from other services;
differences from the original numbers must not be interpreted as citation growth.
The [original February 1, 2025 citation snapshot](citations/README-2025-02-01.md)
is preserved for historical reference.

<table>
    <tr>
        <td>Metrics</td>
        <td>Citation number (OpenAlex, Oct.13,2026)</td>
        <td>Earliest publication time</td>
        <td>With/Without reference</td>
        <td>Paper name</td>
    </tr>
    <tr>
        <td colspan="5" align="center"><a id="1"></a> 📖HVS-Based Method</td>
    </tr>
    <tr>
        <td>signal-to-noise ratio (SNR)</td>
        <td></td>
        <td></td>
        <td>With</td>
        <td></td>
    </tr>
    <tr>
        <td>peak SNR (PSNR)</td>
        <td></td>
        <td></td>
        <td>With</td>
        <td></td>
    </tr>
    <tr>
        <td>mean squared error (MSE)</td>
        <td></td>
        <td></td>
        <td>With</td>
        <td></td>
    </tr>
    <tr>
        <td>structural similarity (SSIM)</td>
        <td><a href="https://openalex.org/W2133665775">57354</a></td>
        <td>2004.04</td>
        <td>With</td>
        <td>
          <a href="https://ieeexplore.ieee.org/document/1284395">Image quality assessment: From error visibility to structural similarity</a>
        </td>
    </tr>
    <tr>
        <td>multi-scale SSIM (MS-SSIM)</td>
        <td><a href="https://openalex.org/W1580389772">5888</a></td>
        <td>2004.05</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/document/1292216">Multiscale structural similarity for image quality assessment</a></td>
    </tr>
    <tr>
        <td>universal image quality index (UQI)</td>
        <td><a href="https://openalex.org/W2159269332">5732</a></td>
        <td>2002.03</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/document/995823">A universal image quality index</a></td>
    </tr>
    <tr>
        <td>feature similarity index (FSIM)</td>
        <td><a href="https://openalex.org/W2141983208">5195</a></td>
        <td>2011.01</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/document/5705575">FSIM: A feature similarity index for image quality assessment</a></td>
    </tr>
    <tr>
        <td>Visual information fidelity (VIF)</td>
        <td><a href="https://openalex.org/W2046119925">4082</a></td>
        <td>2006.02</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/abstract/document/1576816">Image information and visual quality</a></td>
    </tr>
    <tr>
        <td>Most Apparent Distortion (MAD)</td>
        <td><a href="https://openalex.org/W2171349048">1945</a></td>
        <td>2010.01</td>
        <td>With</td>
        <td><a href="https://s2.smu.edu/~eclarson/pubs/2010JEI_MAD.pdf">Most apparent distortion: Full-reference image quality assessment and the role of strategy</a></td>
    </tr>
    <tr>
        <td>Gradient Magnitude Similarity Deviation (GMSD)</td>
        <td><a href="https://openalex.org/W1964859077">1684</a></td>
        <td>2013.12</td>
        <td>With</td>
        <td><a href="https://arxiv.org/abs/1308.3052">Gradient magnitude similarity deviation: A highly efficient perceptual image quality index</a></td>
    </tr>
    <tr>
        <td>Visual SNR (VSNR)</td>
        <td><a href="https://openalex.org/W2009272644">1146</a></td>
        <td>2007.08</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/document/4286985">VSNR: A wavelet-based visual signal-to-noise ratio for natural images</a></td>
    </tr>
    <tr>
        <td>Information content Weighted SSIM (IW-SSIM)</td>
        <td><a href="https://openalex.org/W2114582993">1298</a></td>
        <td>2010.11</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/document/5635337">Information content weighting for perceptual image quality assessment</a></td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W2158564760">786</a></td>
        <td>2002.05</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/abstract/document/5745362">Why is image quality assessment so difficult?</a></td>
    </tr>
    <tr>
        <td>Visual Saliency-induced Index(VSI)</td>
        <td><a href="https://openalex.org/W2015196405">1026</a></td>
        <td>2014.08</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/document/6873260">VSI: A visual saliency-induced index for perceptual image quality assessment</a></td>
    </tr>
    <tr>
        <td>GSIM</td>
        <td><a href="https://openalex.org/W1972006393">701</a></td>
        <td>2011.11</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/abstract/document/6081939">Image quality assessment based on gradient similarity</a></td>
    </tr>
    <tr>
        <td>complex wavelets-SSIM (CW-SSIM)</td>
        <td><a href="https://openalex.org/W2130414230">283</a></td>
        <td>2005.05</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/document/1415469">Translation insensitive image similarity in complex wavelet domain</a></td>
    </tr>
    <tr>
        <td>HVS-based peak SNR (PSNR-HVS)</td>
        <td><a href="https://openalex.org/W2729302458">239</a></td>
        <td>2006.01</td>
        <td>With</td>
        <td><a href="https://www.researchgate.net/publication/251229783_A_NEW_FULL-REFERENCE_QUALITY_METRICS_BASED_ON_HVS">A new full-reference quality metrics based on HVS</a></td>
    </tr>
    <tr>
        <td>RR-SSIM</td>
        <td><a href="https://openalex.org/W1971155098">272</a></td>
        <td>2012.08</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/document/6193206">Reduced-reference image quality assessment by structural similarity estimation</a></td>
    </tr>
    <tr>
        <td>PSIM</td>
        <td><a href="https://openalex.org/W2579658395">237</a></td>
        <td>2017.05</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/abstract/document/7815393">A fast reliable image quality predictor by fusing micro- and macro-structures</a></td>
    </tr>
    <tr>
        <td colspan="5" align="center"><a id="2"></a> 📖Transform Domain-Based Method</td>
    </tr>
    <tr>
        <td>BLIINDS-II</td>
        <td><a href="https://openalex.org/W2162692770">1750</a></td>
        <td>2012.03</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/document/6172573">Blind image quality assessment: A natural scene statistics approach in the DCT domain</a></td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W2153582625">430</a></td>
        <td>2005.03</td>
        <td>With</td>
        <td><a href="https://www.semanticscholar.org/paper/Reduced-reference-image-quality-assessment-using-a-Wang-Simoncelli/7fabaa7282d758159611eeac373a3374dbd855dc">Reduced-reference image quality assessment using a wavelet-domain natural image statistic model</a></td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W2167349140">323</a></td>
        <td>2006.02</td>
        <td></td>
        <td><a href="https://ieeexplore.ieee.org/document/1576815">An SVD-based grayscale image quality measure for local and global assessment</a></td>
    </tr>
    <tr>
        <td>SFF</td>
        <td><a href="https://openalex.org/W2005001434">158</a></td>
        <td>2013.06</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/document/6525380">Sparse feature fidelity for perceptual image quality assessment</a></td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W2007795666">42</a></td>
        <td>2015.07</td>
        <td>With</td>
        <td><a href="https://www.sciencedirect.com/science/article/pii/S0925231215001253">Image quality assessment: a sparse learning way</a></td>
    </tr>
    <tr>
        <td>QASD</td>
        <td><a href="https://openalex.org/W2410760478">44</a></td>
        <td>2016.06</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/document/7486021#:~:text=In%20this%20paper%2C%20a%20new%20sparse%20representation-based%20image,proposed%20based%20on%20the%20construction%20of%20adaptive%20sub-dictionaries.">Sparse representation-based image quality index with adaptive sub-dictionaries</a></td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W2767913386">44</a></td>
        <td>2017.11</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/document/8101526">From sparse coding significance to perceptual quality: a new approach for image quality assessment</a></td>
    </tr>
    <tr>
        <td colspan="5" align="center"><a id="3"></a> 📖NSS-Based Method</td>
    </p></tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W2161907179">2964</a></td>
        <td>2006.10</td>
        <td></td>
        <td><a href="https://ieeexplore.ieee.org/document/1709988">A statistical evaluation of recent full reference image quality assessment algorithms</a></td>
    </tr>
    <tr>
        <td>IFC</td>
        <td><a href="https://openalex.org/W2142884912">1396</a></td>
        <td>2005.11</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/document/1532311">An information fidelity criterion for image quality assessment using natural scene statistics</a></td>
    </tr>
    <tr>
        <td>Tone-Mapped images Quality Index (TMQI)</td>
        <td><a href="https://openalex.org/W1976478698">630</a></td>
        <td>2012.10</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/document/6319406">Objective quality assessment of tone-mapped images</a></td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W2119999314">301</a></td>
        <td>2007.09</td>
        <td></td>
        <td><a href="https://www.researchgate.net/publication/5788132_Blind_image_quality_assessment_through_anisotropy">Blind image quality assessment through anisotropy</a></td>
    </tr>
    <tr>
        <td>Dynamic Range Independent quality Measure (DRIM)</td>
        <td> </td>
        <td>2008.08</td>
        <td>With</td>
        <td><a href="https://www.cl.cam.ac.uk/~rkm38/pdfs/aydin08driiqa.pdf">Dynamic range independent image quality assessment</a></td>
    </tr>
    <tr>
        <td colspan="5" align="center"><a id="4"></a> 📖Traditional Machine Learning Method</td>
    </tr>
    <tr>
        <td>BRISQUE</td>
        <td><a href="https://openalex.org/W1982471090">5975</a></td>
        <td>2012.08</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/document/6272356">No-reference image quality assessment in the spatial domain</a></td>
    </tr>
    <tr>
        <td>DIIVINE</td>
        <td><a href="https://openalex.org/W2129644086">1758</a></td>
        <td>2011.01</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/abstract/document/5756237">Blind image quality assessment: From natural scene statistics to perceptual quality</a></td>
    </tr>
    <tr>
        <td>IL-NIQE</td>
        <td><a href="https://openalex.org/W1977725648">1294</a></td>
        <td>2015.04</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/document/7094273">A feature-enriched completely blind image quality evaluator</a></td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W2159311532">227</a></td>
        <td>2009.03</td>
        <td>Without</td>
        <td><a href="https://www.sciencedirect.com/science/article/pii/S1568494608001075">No-reference image quality assessment using modified extreme learning machine classifier</a></td>
    </tr>
    <tr>
        <td>Multi-Method Fusion (MMF)</td>
        <td><a href="https://openalex.org/W2164287382">195</a></td>
        <td>2012.12</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/abstract/document/6392947">Image quality assessment using multi-method fusion</a></td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W2125312659">147</a></td>
        <td>2010.01</td>
        <td></td>
        <td><a href="https://ieeexplore.ieee.org/document/5395628">Objective image quality assessment based on support vector regression</a></td>
    </tr>
    <tr>
        <td>SVDR</td>
        <td><a href="https://openalex.org/W2102817897">152</a></td>
        <td>2011.09</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/document/6031933">SVD-based quality metric for image and video using machine learning</a></td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W2069737080">164</a></td>
        <td>2015.03</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/abstract/document/7060692">Blind Image Quality Assessment Based on Multichannel Feature Fusion and Label Transfer</a></td>
    </tr>
    <tr>
        <td>ParaBoost</td>
        <td><a href="https://openalex.org/W2344482072">92</a></td>
        <td>2015.12</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/document/7358139">A paraboost method to image quality assessment</a></td>
    </tr>
    <tr>
        <td colspan="5" align="center"><a id="5"></a> 📖CNN-Based Method</td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W2962785568">13944</a></td>
        <td>2018.01</td>
        <td></td>
        <td><a href="https://arxiv.org/abs/1801.03924">The Unreasonable Effectiveness of Deep Features as a Perceptual Metric</a></td>
    </tr>
    <tr>
        <td>IQA-CNN</td>
        <td><a href="https://openalex.org/W2051596736">1267</a></td>
        <td>2014.09</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/document/6909620">Convolutional neural networks for no-reference image quality assessment</a></td>
    </tr>
    <tr>
        <td></td>
        <td> </td>
        <td>2017.10</td>
        <td>FR+NR</td>
        <td><a href="https://ieeexplore.ieee.org/document/8063957">Deep neural networks for no-reference and full-reference image quality assessment</a></td>
    </tr>
    <tr>
        <td>DISTS</td>
        <td><a href="https://openalex.org/W3017136408">939</a></td>
        <td>2020.12</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/document/9298952">Image Quality Assessment: Unifying Structure and Texture Similarity</a></td>
    </tr>
    <tr>
        <td>BIQA by a Self-Adaptive<br>Hyper Network</td>
        <td><a href="https://openalex.org/W3035719652">841</a></td>
        <td>2020.06</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/document/9156687">Blindly Assess Image Quality in the Wild Guided by a Self-Adaptive Hyper Network</a></td>
    </tr>
    <tr>
        <td>MEON</td>
        <td><a href="https://openalex.org/W2768340063">619</a></td>
        <td>2017.11</td>
        <td></td>
        <td><a href="https://ieeexplore.ieee.org/document/8110690">End-to-end blind image quality assessment using deep neural networks</a></td>
    </tr>
    <tr>
        <td>RankIQA</td>
        <td><a href="https://openalex.org/W2963975576">513</a></td>
        <td>2017.07</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/document/8237380">RankIQA: Learning from rankings for no-reference image quality assessment</a></td>
    </tr>
    <tr>
        <td>BIECON</td>
        <td><a href="https://openalex.org/W2566149141">458</a></td>
        <td>2016.12</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/document/7782419">Fully deep blind image quality predictor</a></td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W2170947705">368</a></td>
        <td>2014.08</td>
        <td></td>
        <td><a href="https://ieeexplore.ieee.org/document/6872541">Blind image quality assessment via deep learning</a></td>
    </tr>
    <tr>
        <td>DeepBIQ</td>
        <td><a href="https://openalex.org/W2286686646">277</a></td>
        <td>2016.02</td>
        <td>Without</td>
        <td><a href="https://arxiv.org/abs/1602.05531">On the use of deep learning for blind image quality assessment</a></td>
    </tr>
    <tr>
        <td>Deep image Quality Assessment (DeepQA)</td>
        <td><a href="https://openalex.org/W2737134362">264</a></td>
        <td>2017.10</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/abstract/document/8099696">Deep learning of human visual sensitivity in image quality assessment framework</a></td>
    </tr>
    <tr>
        <td>DeepSim</td>
        <td><a href="https://openalex.org/W2586275201">172</a></td>
        <td>2017.09</td>
        <td>With</td>
        <td><a href="https://www.sciencedirect.com/science/article/pii/S0925231217301480">DeepSim: deep similarity for image quality assessment</a></td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W2052287864">94</a></td>
        <td>2014.09</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/document/6909764">Blind image quality assessment using semi-supervised rectifier networks</a></td>
    </tr>
    <tr>
        <td>Re-IQA</td>
        <td><a href="https://openalex.org/W4386071753">144</a></td>
        <td>2023.04</td>
        <td>Without</td>
        <td><a href="https://arxiv.org/abs/2304.00451">Re-IQA: Unsupervised Learning for Image Quality Assessment in the Wild</a></td>
    </tr>
    <tr>
        <td>Multi-Pooled Inception Features for NR IQA</td>
        <td><a href="https://openalex.org/W3014019158">37</a></td>
        <td>2020.02</td>
        <td>Without</td>
        <td><a href="https://www.mdpi.com/2076-3417/10/6/2186">Multi-Pooled Inception Features for No-Reference Image Quality Assessment</a></td>
    </tr>
    <tr>
        <td>IQMA Network</td>
        <td><a href="https://openalex.org/W3175517129">24</a></td>
        <td>2021.06</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/document/9523177">IQMA Network: Image Quality Multi-Scale Assessment Network</a></td>
    </tr>
    <tr>
        <td colspan="5" align="center"><a id="6"></a> 📖Transformer-Based Method</td>
    </tr>
    <tr>
        <td>MUSIQ</td>
        <td><a href="https://openalex.org/W3201711438">950</a></td>
        <td>2021.08</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/document/9710973">MUSIQ: Multi-Scale Image Quality Transformer</a></td>
    </tr>
    <tr>
        <td>ViT with relative ranking<br>and self-consistency</td>
        <td><a href="https://openalex.org/W3194280054">444</a></td>
        <td>2021.08</td>
        <td>Without</td>
        <td><a href="https://arxiv.org/abs/2108.06858">No-reference image quality assessment via transformers, relative ranking,and self-consistency</a></td>
    </tr>
    <tr>
        <td>Maniqa</td>
        <td> </td>
        <td>2022.04</td>
        <td>Without</td>
        <td><a href="https://arxiv.org/abs/2204.08958">Maniqa: Muli-dimension attention network for no-reference image quality assessment</a></td>
    </tr>
    <tr>
        <td>TRIQ</td>
        <td> </td>
        <td>2020.12</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/abstract/document/9506075">Transformer for Image Quality Assessment</a></td>
    </tr>
    <tr>
        <td>IQT</td>
        <td><a href="https://openalex.org/W3176622443">168</a></td>
        <td>2021.04</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/document/9523022">Perceptual Image Quality Assessment With Transformers</a></td>
    </tr>
    <tr>
        <td>NTIRE 2021 Challenge<br>on Perceptual IQA</td>
        <td><a href="https://openalex.org/W3174760001">55</a></td>
        <td>2021.05</td>
        <td></td>
        <td><a href="https://arxiv.org/abs/2105.03072">NTIRE 2021 Challenge on Perceptual Image Quality Assessment</a></td>
    </tr>
    <tr>
        <td>NTIRE 2022 Challenge<br>on Perceptual IQA</td>
        <td> </td>
        <td>2022.06</td>
        <td></td>
        <td><a href="https://arxiv.org/abs/2206.11695">NTIRE 2022 Challenge on Perceptual Image Quality Assessment</a></td>
    </tr>
    <tr>
        <td>Jacobian Lens Distance (JLD)</td>
        <td></td>
        <td>2026.10</td>
        <td>With</td>
        <td><a href="https://arxiv.org/abs/2610.05967">JLD: Perceptual Distance Through A Jacobian Lens</a></td>
    </tr>
    <tr>
        <td colspan="5" align="center"><a id="7"></a> 📖Framework-Based Method</td>
    </tr>
    <tr>
        <td>QAC</td>
        <td><a href="https://openalex.org/W2162915697">404</a></td>
        <td>2013.06</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/document/6618977">Learning without human scores for blind image quality assessment</a></td>
    </tr>
    <tr>
        <td>MetalQA</td>
        <td> </td>
        <td>2020.04</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/document/9156932">MetalQA: Deep Meta-Learning for No-Reference Image Quality Assessment</a></td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W2807793257">331</a></td>
        <td>2018.06</td>
        <td></td>
        <td><a href="https://ieeexplore.ieee.org/document/8383698">Deep CNN-based blind image quality predictor</a></td>
    </tr>
    <tr>
        <td>UNIQUE</td>
        <td><a href="https://openalex.org/W3030380536">325</a></td>
        <td>2021.03</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/abstract/document/9369977">Uncertainty-Aware Blind Image Quality Assessment in the Laboratory and Wild</a></td>
    </tr>
    <tr>
        <td>Hallucinated-IQA</td>
        <td><a href="https://openalex.org/W2964065910">264</a></td>
        <td>2018.04</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/document/8578181">Hallucinated-IQA: No-reference image quality assessment via adversarial learning</a></td>
    </tr>
    <tr>
        <td>CONTRIQUE</td>
        <td><a href="https://openalex.org/W3210514413">284</a></td>
        <td>2022.06</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/document/9796010">Image quality assessment using contrastive learning</a></td>
    </tr>
    <tr>
        <td>DeepFL-IQA</td>
        <td><a href="https://openalex.org/W3000809580">31</a></td>
        <td>2020.01</td>
        <td>Without</td>
        <td><a href="https://arxiv.org/abs/2001.08113">DeepFL-IQA: Weak Supervision for Deep IQA Feature Learning</a></td>
    </tr>
    <tr>
        <td>CVRDK-IQA</td>
        <td><a href="https://openalex.org/W4221144351">49</a></td>
        <td>2022.02</td>
        <td>Without</td>
        <td><a href="https://arxiv.org/abs/2202.13123">Content-Variant Reference Image Quality Assessment via Knowledge Distillation</a></td>
    </tr>
    <tr>
        <td>CNN-Based Medical<br>Ultrasound IQA</td>
        <td><a href="https://openalex.org/W3176592499">29</a></td>
        <td>2021.07</td>
        <td>Without</td>
        <td><a href="https://www.researchgate.net/publication/355377889_CNN-Based_Medical_Ultrasound_Image_Quality_Assessment">CNN-Based Medical Ultrasound Image Quality Assessment</a></td>
    </tr>
    <tr>
        <td colspan="5" align="center"><a id="8"></a> 📖Medical IQA</td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W2783148479">429</a></td>
        <td>2018.04</td>
        <td>Without</td>
        <td><a href="https://www.sciencedirect.com/science/article/pii/S1053811917310832">Quantitative assessment of structural image quality</a></td>
    </tr>
    <tr>
        <td colspan="5" align="center"><a id="9"></a> 📖IQA for Dehazing Algorithm</td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W2918431349">252</a></td>
        <td>2019.02</td>
        <td>With</td>
        <td><a href="https://ieeexplore.ieee.org/abstract/document/8654007">Quality evaluation of image dehazing methods using synthetic hazy images</a></td>
    </tr>
    <tr>
        <td colspan="5" align="center"><a id="10"></a> 📖Portrait Quality Assessment</td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W4402916241">16</a></td>
        <td>2024.04</td>
        <td>Without</td>
        <td><a href="https://arxiv.org/abs/2404.11159">Deep Portrait Quality Assessment. A NTIRE 2024 Challenge Survey</a></td>
    </tr>
    <tr>
        <td colspan="5" align="center"><a id="11"></a> 📖IQA for Low Light Enhancement</td>
    </tr>
    <tr>
        <td>NLIEE</td>
        <td><a href="https://openalex.org/W3171407434">47</a></td>
        <td>2021.06</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/document/9428312">A no-reference evaluation metric for low-light image enhancement</a></td>
    </tr>
    <tr>
        <td colspan="5" align="center"><a id="12"></a> 📖Specific Distortion</td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W2138088051">759</a></td>
        <td>2009.04</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/document/4799375">A no-reference objective image sharpness metric based on the notion of just noticeable blur (JNB)</a></td>
    </tr>
    <tr>
        <td>BIBLE</td>
        <td><a href="https://openalex.org/W1978598038">270</a></td>
        <td>2015.01</td>
        <td>Without</td>
        <td><a href="https://ieeexplore.ieee.org/document/7027178">No-reference image blur assessment based on discrete orthogonal moments</a></td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W2015015901">101</a></td>
        <td>2013.11</td>
        <td></td>
        <td><a href="https://dl.acm.org/doi/10.1145/2508363.2508391">A no-reference metric for evaluating the quality of motion deblurring</a></td>
    </tr>
    <tr>
        <td></td>
        <td><a href="https://openalex.org/W1997826598">22</a></td>
        <td>2015.02</td>
        <td>Without</td>
        <td><a href="https://www.sciencedirect.com/science/article/pii/S1434841114002519">Full reference image quality metrics for JPEG compressed images</a></td>
    </tr>
</table>

## 👨‍💻 Contributers
 - Zhengyi Shi@[11xiaoyi11](https://github.com/11xiaoyi11)
 - Chengqian Ma@[step-out](https://github.com/step-out) 
 - Weixuan Jin@[axax11344](https://github.com/axax11344) 

## 💡 Citation
If you find this survey useful, please cite our paper:
```
@misc{ma2025surveyimagequalityassessment,
      title={A Survey on Image Quality Assessment: Insights, Analysis, and Future Outlook}, 
      author={Chengqian Ma and Zhengyi Shi and Zhiqiang Lu and Shenghao Xie and Fei Chao and Yao Sui},
      year={2025},
      eprint={2502.08540},
      archivePrefix={arXiv},
      primaryClass={cs.CV},
      url={https://arxiv.org/abs/2502.08540}, 
}
```

## 📧 Contact Us
If you have any questions or suggestions, please contact us via:
- Email: chengqianma@yeah.net, zyshi@stu.xmu.edu.cn
