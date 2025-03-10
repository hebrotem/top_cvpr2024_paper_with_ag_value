[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Fhebrotem%2FTop_Cvpr2024_Paper_with_Ag_value&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=Page+visitors&edge_flat=false)](https://hits.seeyoufarm.com)
<!-- ![Hello badge](https://visitor-badge.laobi.icu/badge?page_id=hebrotem.Top_Cvpr2024_Paper_with_Ag_value)

<div align="center">
  <h1 align="center">Top CVPR 2024 Papers with Agriculture Application Values </h1>
  <a href="https://github.com/SkalskiP/top-cvpr-2023-papers">2023</a>
</div>
-->
<br>

<!--
<div align="center">
  <img width="600" src="https://github.com/SkalskiP/top-cvpr-2024-papers/assets/26109316/347853f9-9e93-4ca0-858b-a7c3f6bba073" alt="vancouver">
</div>
-->

## 👋 hello
> Computer Vision and Pattern Recognition (CVPR) is a major conference, and in 2024, it received 11,532 paper submissions, 
> out of which 2,719 were accepted. I've created this repository to help you find not only the best from CVPR publications, but also those extendable to agricultural domain. 
> If the paper you seek isn't in my curated list, feel free to check out the full [list](https://cvpr.thecvf.com/Conferences/2024/AcceptedPapers) of accepted papers.

# 【CVPR 2024 Papers Extendable to Agriculture】

<details> <summary><strong>List of Papers</strong></summary>
    
  - [Image and video synthesis and generation](#Image-and-video-synthesis-and-generation)
  - [3D from multi-view and sensors](#3DfromMulti)
  - [Deep learning architectures and techniques](#Deeplearning)
  - [Document analysis and understanding](Documentanalysis)

</details>

---
<a name="Image-and-video-synthesis-and-generation"></a>
### Image and video synthesis and generation
- <p align="left">
    <a href="https://arxiv.org/abs/2309.11497" title="FreeU: Free Lunch in Diffusion U-Net">
       <strong>FreeU: Free Lunch in Diffusion U-Net</strong>
    </a>
    <br/>
    Authors: Chenyang Si, Ziqi Huang, Yuming Jiang, Ziwei Liu
    <br/>
    <a href="https://arxiv.org/abs/2403.14602"><img src="https://img.shields.io/badge/arXiv-FreeU-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Si_FreeU_Free_Lunch_in_Diffusion_U-Net_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://github.com/ChenyangSi/FreeU"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://chenyangsi.top/FreeU/"><img src="https://img.shields.io/badge/Project_Page-FreeU-blue' alt='Project Page"></a> <a href="https://www.youtube.com/watch?v=eFmkJ_oEW5s"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a>
  <details> <summary><strong>Abstract</strong></summary>
      In this paper, we uncover the untapped potential of diffusion U-Net, which serves as a "free lunch" that substantially improves the generation quality on the fly. We initially investigate the key contributions of the U-Net architecture to the denoising process and identify that its main backbone primarily contributes to denoising, whereas its skip connections mainly introduce high-frequency features into the decoder module, causing the network to overlook the backbone semantics. Capitalizing on this discovery, we propose a simple yet effective method-termed "FreeU" - that enhances generation quality without additional training or finetuning. Our key insight is to strategically re-weight the contributions sourced from the U-Net's skip connections and backbone feature maps, to leverage the strengths of both components of the U-Net architecture. Promising results on image and video generation tasks demonstrate that our FreeU can be readily integrated to existing diffusion models, e.g., Stable Diffusion, DreamBooth, ModelScope, Rerender and ReVersion, to improve the generation quality with only a few lines of code. All you need is to adjust two scaling factors during inference. 
    </details>
    <strong>Likely application in agriculture:</strong> Data augmentation
</p>

- <p align="left">
    <a href="https://arxiv.org/abs/2402.19481" title="DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models">
       <strong>DistriFusion: Distributed Parallel Inference for High-Resolution Diffusion Models</strong>
    </a>
    <br/>
    Muyang Li, Tianle Cai, Jiaxin Cao, Qinsheng Zhang, Han Cai, Junjie Bai, Yangqing Jia, Kai Li, Song Han
    <br/>
    <a href="https://arxiv.org/abs/2402.19481"><img src="https://img.shields.io/badge/arXiv-distriFusion-b31b1b.svg" height=20.5></a> <a href="href="https://openaccess.thecvf.com/content/CVPR2024/papers/Li_DistriFusion_Distributed_Parallel_Inference_for_High-Resolution_Diffusion_Models_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://github.com/mit-han-lab/distrifuser"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://hanlab.mit.edu/projects/distrifusion"><img src="https://img.shields.io/badge/Project_Page-DistriFusion-blue' alt='Project Page"></a> <a href="https://www.youtube.com/watch?v=EZX7srDDmW0"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a>
    <details> <summary><strong>Abstract</strong></summary>
      Diffusion models have achieved great success in synthesizing high-quality images. However, generating high-resolution images with diffusion models is still challenging due to the enormous computational costs, resulting in a prohibitive latency for interactive applications. In this paper, we propose DistriFusion to tackle this problem by leveraging parallelism across multiple GPUs. Our method splits the model input into multiple patches and assigns each patch to a GPU. However, naively implementing such an algorithm breaks the interaction between patches and loses fidelity, while incorporating such an interaction will incur tremendous communication overhead. To overcome this dilemma, we observe the high similarity between the input from adjacent diffusion steps and propose displaced patch parallelism, which takes advantage of the sequential nature of the diffusion process by reusing the pre-computed feature maps from the previous timestep to provide context for the current step. Therefore, our method supports asynchronous communication, which can be pipelined by computation. Extensive experiments show that our method can be applied to recent Stable Diffusion XL with no quality degradation and achieve up to a 6.1× speedup on eight NVIDIA A100s compared to one.
    </details>
    <strong>Likely application in agriculture:</strong> Data augmentation
</p>

- <p align="left">
    <a href="https://arxiv.org/abs/2312.15540" title="Amodal Completion via Progressive Mixed Context Diffusion">
       <strong>Amodal Completion via Progressive Mixed Context Diffusion</strong>
    </a>
    <br/>
    Katherine Xu, Lingzhi Zhang, Jianbo Shi
    <br/>
    <a href="https://arxiv.org/abs/2312.15540"><img src="https://img.shields.io/badge/arXiv-Amodal-b31b1b.svg" height=20.5></a> <a href="href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xu_Amodal_Completion_via_Progressive_Mixed_Context_Diffusion_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://github.com/k8xu/amodal"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://k8xu.github.io/amodal/"><img src="https://img.shields.io/badge/Project_Page-Amodal-blue' alt='Project Page"></a> <!-- <a href="https://www.youtube.com/watch?v=EZX7srDDmW0"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> -->
    <details> <summary><strong>Abstract</strong></summary>
      Our brain can effortlessly recognize objects even when partially hidden from view. Seeing the visible of the hidden is called amodal completion; however, this task remains a challenge for generative AI despite rapid progress. We propose to sidestep many of the difficulties of existing approaches, which typically involve a two-step process of predicting amodal masks and then generating pixels. Our method involves thinking outside the box, literally! We go outside the object bounding box to use its context to guide a pre-trained diffusion inpainting model, and then progressively grow the occluded object and trim the extra background. We overcome two technical challenges: 1) how to be free of unwanted co-occurrence bias, which tends to regenerate similar occluders, and 2) how to judge if an amodal completion has succeeded. Our amodal completion method exhibits improved photorealistic completion results compared to existing approaches in numerous successful completion cases. And the best part? It doesn't require any special training or fine-tuning of models.
    </details>
    <strong>Likely application in agriculture:</strong> Occlusion-aware amodal Completion
</p>

- <p align="left">
    <a href="https://arxiv.org/abs/2405.20324" title="Don't Drop Your Samples! Coherence-Aware Training Benefits Conditional Diffusion">
       <strong>Don't Drop Your Samples! Coherence-Aware Training Benefits Conditional Diffusion</strong>
    </a>
    <br/>
    Nicolas Dufour, Victor Besnier, Vicky Kalogeiton, David Picard
    <br/>
    <a href="https://arxiv.org/abs/2405.20324"><img src="https://img.shields.io/badge/arXiv-Don't Drop-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Dufour_Dont_Drop_Your_Samples_Coherence-Aware_Training_Benefits_Conditional_Diffusion_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://github.com/nicolas-dufour/CAD"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://nicolas-dufour.github.io/cad"><img src="https://img.shields.io/badge/Project_Page-Don't_Drop-blue' alt='Project Page"></a> <a href="https://www.youtube.com/watch?v=4Tu-x2-Zcxs"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a>
    <details> <summary><strong>Abstract</strong></summary>
      Conditional diffusion models are powerful generative models that can leverage various types of conditional information, such as class labels, segmentation masks, or text captions. However, in many real-world scenarios, conditional information may be noisy or unreliable due to human annotation errors or weak alignment. In this paper, we propose the Coherence-Aware Diffusion (CAD), a novel method that integrates coherence in conditional information into diffusion models, allowing them to learn from noisy annotations without discarding data. We assume that each data point has an associated coherence score that reflects the quality of the conditional information. We then condition the diffusion model on both the conditional information and the coherence score. In this way, the model learns to ignore or discount the conditioning when the coherence is low. We show that CAD is theoretically sound and empirically effective on various conditional generation tasks. Moreover, we show that leveraging coherence generates realistic and diverse samples that respect conditional information better than models trained on cleaned datasets where samples with low coherence have been discarded.
    </details>
    <strong>Likely application in agriculture:</strong> Deep data augmentation
</p>

- <p align="left">
    <a href="https://arxiv.org/abs/2312.06038" title="Correcting Diffusion Generation through Resampling">
       <strong>Correcting Diffusion Generation through Resampling</strong>
    </a>
    <br/>
    Yujian Liu, Yang Zhang, Tommi Jaakkola, Shiyu Chang
    <br/>
    <a href="https://arxiv.org/abs/2312.06038"><img src="https://img.shields.io/badge/arXiv-Correcting-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Liu_Correcting_Diffusion_Generation_through_Resampling_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://github.com/UCSB-NLP-Chang/diffusion_resampling"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://nicolas-dufour.github.io/cad"><img src="https://img.shields.io/badge/Project_Page-Correcting-blue' alt='Project Page"></a> <a href="https://www.youtube.com/watch?v=4Tu-x2-Zcxs"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a>
    <details> <summary><strong>Abstract</strong></summary>
      Despite diffusion models' superior capabilities in modeling complex distributions, there are still non-trivial distributional discrepancies between generated and ground-truth images, which has resulted in several notable problems in image generation, including missing object errors in text-to-image generation and low image quality. Existing methods that attempt to address these problems mostly do not tend to address the fundamental cause behind these problems, which is the distributional discrepancies, and hence achieve sub-optimal results. In this paper, we propose a particle filtering framework that can effectively address both problems by explicitly reducing the distributional discrepancies. Specifically, our method relies on a set of external guidance, including a small set of real images and a pre-trained object detector, to gauge the distribution gap, and then design the resampling weight accordingly to correct the gap. Experiments show that our methods can effectively correct missing object errors and improve image quality in various image generation tasks. Notably, our method outperforms the existing strongest baseline by 5% in object occurrence and 1.0 in FID on MS-COCO.
    </details>
    <strong>Likely application in agriculture:</strong> Text-conditioned image generation
</p>

- <p align="left">
    <a href="https://arxiv.org/abs/2311.17002" title="Ranni: Taming Text-to-Image Diffusion for Accurate Instruction Following">
    <strong>Ranni: Taming Text-to-Image Diffusion for Accurate Instruction Following </strong>
    </a>
    <br/>
    Yutong Feng, Biao Gong, Di Chen, Yujun Shen, Yu Liu, Jingren Zhou
    <br/>
    <a href="https://arxiv.org/abs/2311.17002"><img src="https://img.shields.io/badge/arXiv-Ranni-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Feng_Ranni_Taming_Text-to-Image_Diffusion_for_Accurate_Instruction_Following_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://github.com/ali-vilab/Ranni"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href='https://ranni-t2i.github.io/Ranni/'><img src="https://img.shields.io/badge/Project_Page-Ranni-blue' alt='Project Page"></a> <a href="https://www.youtube.com/watch?v=1IIat83Atjk"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5> </a> 
    <details> <summary><strong>Abstract</strong></summary>
      Existing text-to-image (T2I) diffusion models usually struggle in interpreting complex prompts, especially those with quantity, object-attribute binding, and multi-subject descriptions. In this work, we introduce a semantic panel as the middleware in decoding texts to images, supporting the generator to better follow instructions. The panel is obtained through arranging the visual concepts parsed from the input text by the aid of large language models, and then injected into the denoising network as a detailed control signal to complement the text condition. To facilitate text-to-panel learning, we come up with a carefully designed semantic formatting protocol, accompanied by a fully-automatic data preparation pipeline. Thanks to such a design, our approach, which we call Ranni, manages to enhance a pre-trained T2I generator regarding its textual controllability. More importantly, the introduction of the generative middleware brings a more convenient form of interaction (i.e., directly adjusting the elements in the panel or using language instructions) and further allows users to finely customize their generation, based on which we develop a practical system and showcase its potential in continuous generation and chatting-based editing.
    </details>
    <strong>Likely application in agriculture:</strong> Text-to-Image
</p>

<!--- - <p align="left">
    <a href="https://arxiv.org/abs/2312.02149" title="Don't Drop Your Samples! Coherence-Aware Training Benefits Conditional Diffusion">
       <strong>Generative Powers of Ten</strong>
    </a>
    <br/>
    Xiaojuan Wang, Janne Kontkanen, Brian Curless, Steve Seitz, Ira Kemelmacher, Ben Mildenhall, Pratul Srinivasan, Dor Verbin, Aleksander Holynski
    <br/>
    <a href="https://arxiv.org/abs/2312.02149"><img src="https://img.shields.io/badge/arXiv-Gen Ten-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Wang_Generative_Powers_of_Ten_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://powers-of-10.github.io/"><img src="https://img.shields.io/badge/Project_Page-Generative-blue' alt='Project Page"></a>  <a href="https://www.youtube.com/watch?v=0fKBhvDjuy0"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a>

    <strong>Likely application in agriculture:</strong> Text-to-image
</p>

- <p align="left">
    <a href="https://arxiv.org/abs/2406.07480" title="Image Neural Field Diffusion Models">
       <strong>Image Neural Field Diffusion Models</strong>
    </a>
    <br/>
    Yinbo Chen, Oliver Wang, Richard Zhang, Eli Shechtman, Xiaolong Wang, Michael Gharbi
    <br/>
    <a href="https://arxiv.org/abs/2406.07480"><img src="https://img.shields.io/badge/arXiv-Image Neural-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Chen_Image_Neural_Field_Diffusion_Models_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://yinboc.github.io/infd/"><img src="https://img.shields.io/badge/Project_Page-Generative-blue' alt='Project Page"></a>
    <br/>
    <strong>Likely application in agriculture:</strong> Deep data augmentation
</p>
-->
- <p align="left">
    <a href="https://arxiv.org/abs/2403.01852" title="PLACE: Adaptive Layout-Semantic Fusion for Semantic Image Synthesis">
       <strong>PLACE: Adaptive Layout-Semantic Fusion for Semantic Image Synthesis</strong>
    </a>
    <br/>
    Zhengyao Lv, Yuxiang Wei, Wangmeng Zuo2, Kwan-Yee K. Wong
    <br/>
    <a href="https://arxiv.org/abs/2403.01852"><img src="https://img.shields.io/badge/arXiv-PLACE-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Lv_PLACE_Adaptive_Layout-Semantic_Fusion_for_Semantic_Image_Synthesis_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://github.com/cszy98/PLACE"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://cszy98.github.io/PLACE/"><img src="https://img.shields.io/badge/Project_Page-PLACE-blue' alt='Project Page"></a> <a href="https://www.youtube.com/watch?v=47mMAmclPWw"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a>
    <br/>
    <strong>Likely application in agriculture:</strong> Deep Segmatic image generation
</p>

- <p align="left">
    <a href="https://arxiv.org/abs/2312.02150" title="Readout Guidance: Learning Control from Diffusion Features">
       <strong>Readout Guidance: Learning Control from Diffusion Features</strong>
    </a>
    <br/>
    Grace Luo, Trevor Darrell, Oliver Wang, Dan B Goldman, Aleksander Holynski
    <br/>
    <a href="https://arxiv.org/abs/2312.02150"><img src="https://img.shields.io/badge/arXiv-Readout-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Luo_Readout_Guidance_Learning_Control_from_Diffusion_Features_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://github.com/google-research/readout_guidance"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://readout-guidance.github.io/"><img src="https://img.shields.io/badge/Project_Page-Readout-blue' alt='Project Page"></a> <a href="https://www.youtube.com/watch?v=VoA5WLRN-Oo"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a>
    <br/>
    <strong>Likely application in agriculture:</strong> Deep Segmatic image generation
</p>

- <p align="left">
    <a href="https://arxiv.org/abs/2311.16503" title="TFMQ-DM: Temporal Feature Maintenance Quantization for Diffusion Models">
       <strong>TFMQ-DM: Temporal Feature Maintenance Quantization for Diffusion Models</strong>
    </a>
    <br/>
    Yushi Huang, Ruihao Gong, Jing Liu, Tianlong Chen, Xianglong Liu
  <br/>
    <a href="https://arxiv.org/abs/2311.16503"><img src="https://img.shields.io/badge/arXiv-TFMQ_DM-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Huang_TFMQ-DM_Temporal_Feature_Maintenance_Quantization_for_Diffusion_Models_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://github.com/ModelTC/TFMQ-DM"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://modeltc.github.io/TFMQ-DM/"><img src="https://img.shields.io/badge/Project_Page-TFMQ_DM-blue' alt='Project Page"></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Edge-efficient image generation
</p>

- <p align="left">
    <a href="https://arxiv.org/abs/2404.04650" title="InitNO: Boosting Text-to-Image Diffusion Models via Initial Noise Optimization">
    <strong>InitNO: Boosting Text-to-Image Diffusion Models via Initial Noise Optimization</strong>
    </a>
    <br/>
    Xiefan Guo, Jinlin Liu, Miaomiao Cui, Jiankai Li, Hongyu Yang, Di Huang
  <br/>
    <a href="https://arxiv.org/abs/2404.04650"><img src="https://img.shields.io/badge/arXiv-InitNo-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Guo_InitNO_Boosting_Text-to-Image_Diffusion_Models_via_Initial_Noise_Optimization_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://github.com/xiefan-guo/initno"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://xiefan-guo.github.io/initno/"><img src="https://img.shields.io/badge/Project_Page-InitNO-blue' alt='Project Page"></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Text-to-Image
</p>

<!--- <p align="left">
    <a href="https://arxiv.org/abs/2312.10835" title="Your Student is Better Than Expected: Adaptive Teacher-Student Collaboration for Text-Conditional Diffusion Models">
    <strong>Your Student is Better Than Expected: Adaptive Teacher-Student Collaboration for Text-Conditional Diffusion Models</strong>
    </a>
    <br/>
    Nikita Starodubcev, Dmitry Baranchuk, Artem Fedorov, Artem Babenko
    <br/>
    <a href="https://arxiv.org/abs/2312.10835"><img src="https://img.shields.io/badge/arXiv-InitNo-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Starodubcev_Your_Student_is_Better_Than_Expected_Adaptive_Teacher-Student_Collaboration_for_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://github.com/yandex-research/adaptive-diffusion"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://readout-guidance.github.io/"><img src="https://img.shields.io/badge/Project_Page-Generative-blue' alt='Project Page"></a> <a href="https://www.youtube.com/watch?v=VoA5WLRN-Oo"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a>
    <br/>
    <strong>Likely application in agriculture:</strong> Deep Segmatic image generation
</p> -->


<a name="3DfromMulti"></a>
### 3D from multi-view and sensors

- <p align="left">
    <a href="https://arxiv.org/abs/2304.08069" title="DETRs Beat YOLOs on Real-time Object Detection">
    <strong>DETRs Beat YOLOs on Real-time Object Detection</strong>
    </a>
    <br/>
    Yian Zhao, Wenyu Lv, Shangliang Xu, Jinman Wei, Guanzhong Wang, Qingqing Dang, Yi Liu, Jie Chen
    <br/>
    <a href="https://arxiv.org/abs/2304.08069"><img src="https://img.shields.io/badge/arXiv-DETRs_YOLOs-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Zhao_DETRs_Beat_YOLOs_on_Real-time_Object_Detection_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://github.com/lyuwenyu/RT-DETR"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://zhao-yian.github.io/RTDETR/"><img src="https://img.shields.io/badge/Project_Page-DETRs_YOLOs-blue' alt='Project Page"></a> <a href="https://www.youtube.com/watch?v=UOc0qMSX4Ac"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5> </a> 
    <br/>
    <strong>Likely application in agriculture:</strong> disease detection
</p>

- <p align="left">
    <a href="https://arxiv.org/abs/2312.01220" title="Boosting Object Detection with Zero-Shot Day-Night Domain Adaptation">
       <strong>Boosting Object Detection with Zero-Shot Day-Night Domain Adaptation</strong>
    </a>
    <br/>
    Zhipeng Du, Miaojing Shi, Jiankang Deng
    <br/>
    <a href="https://arxiv.org/abs/2312.01220"><img src="https://img.shields.io/badge/arXiv-Boosting-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Du_Boosting_Object_Detection_with_Zero-Shot_Day-Night_Domain_Adaptation_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://github.com/ZPDu/DAI-Net"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://zpdu.github.io/DAINet_page/"><img src="https://img.shields.io/badge/Project_Page-Boosting-blue' alt='Project Page"></a> <a href="https://www.youtube.com/watch?v=X44b2lInZzk"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5> </a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Disease detection
</p>

- <p align="left">
    <a href="https://arxiv.org/abs/2404.04319" title="SpatialTracker: Tracking Any 2D Pixels in 3D Space">
       <strong>SpatialTracker: Tracking Any 2D Pixels in 3D Space</strong>
    </a>
    <br/>
    Yuxi Xiao, Qianqian Wang, Shangzhan Zhang, Nan Xue, Sida Peng, Yujun Shen, Xiaowei Zhou
    <br/>
    <a href="https://arxiv.org/abs/2404.04319"><img src="https://img.shields.io/badge/arXiv-SpaTracker-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_SpatialTracker_Tracking_Any_2D_Pixels_in_3D_Space_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://github.com/henry123-boy/SpaTracker"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://henry123-boy.github.io/SpaTracker/"><img src="https://img.shields.io/badge/Project_Page-SpaTracker-blue' alt='Project Page"></a> <a href="https://www.youtube.com/watch?v=Z6TcrGf97mM"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5> </a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Trajectory prediction
</p>

- <p align="left">
    <a href="https://arxiv.org/abs/2402.08359" title="Learning to Produce Semi-dense Correspondences for Visual Localization">
    <strong>Learning to Produce Semi-dense Correspondences for Visual Localization</strong>
    </a>
    <br/>
    Khang Truong Giang, Soohwan Song, Sungho Jo
    <br/>
    <a href="https://arxiv.org/abs/2402.08359"><img src="https://img.shields.io/badge/arXiv-DeViLoc-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Giang_Learning_to_Produce_Semi-dense_Correspondences_for_Visual_Localization_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://github.com/TruongKhang/DeViLoc"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://www.youtube.com/watch?v=1z_fvbr1im4"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
  <br/>
  <strong>Likely application in agriculture:</strong> Agricultural robot localization
  </p>

- <p align="left">
    <a href="https://arxiv.org/abs/2311.11013" title="Implicit Event-RGBD Neural SLAM">
    <strong>Implicit Event-RGBD Neural SLAM</strong>
    </a>
    <br/>
    Delin Qu, Chi Yan, Dong Wang, Jie Yin, Dan Xu, Bin Zhao, Xuelong Li
    <br/>
    <a href="https://arxiv.org/abs/2311.11013"><img src="https://img.shields.io/badge/arXiv-ENSLAM-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Qu_Implicit_Event-RGBD_Neural_SLAM_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>

- <p align="left">
    <a href="https://arxiv.org/abs/2311.11013" title="Implicit Event-RGBD Neural SLAM">
    <strong>Implicit Event-RGBD Neural SLAM</strong>
    </a>
    <br/>
    Delin Qu, Chi Yan, Dong Wang, Jie Yin, Dan Xu, Bin Zhao, Xuelong Li
    <br/>
    <a href="https://arxiv.org/abs/2311.11013"><img src="https://img.shields.io/badge/arXiv-ENSLAM-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Qu_Implicit_Event-RGBD_Neural_SLAM_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href="https://github.com/DelinQu/EN-SLAM"><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>

<a name="Deeplearning"></a>
### Deep learning architectures and techniques

- <p align="left">
    <a href="https://arxiv.org/pdf/2311.06242" title="Florence-2: Advancing a Unified Representation for a Variety of Vision Tasks">
        <strong>Florence-2: Advancing a Unified Representation for a Variety of Vision Tasks</strong>
    </a>
    <br/>
    Bin Xiao, Haiping Wu, Weijian Xu, Xiyang Dai, Houdong Hu, Yumao Lu, Michael Zeng, Ce Liu, Lu Yuan
    <br/>
    [<a href="https://arxiv.org/pdf/2311.06242">paper</a>]  [<a href="https://youtu.be/cOlyA00K1ec">video</a>] [<a href="https://huggingface.co/spaces/gokaygokay/Florence-2">demo</a>] [<a href="https://youtu.be/cOlyA00K1ec">colab</a>]
    <br/>
  <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>

<a name="Documentanalysis"></a>
### Document analysis and understanding

- <p align="left">
    <a href="https://arxiv.org/abs/2405.04408" title="DocRes: A Generalist Model Toward Unifying Document Image Restoration Tasks">
        <strong>DocRes: A Generalist Model Toward Unifying Document Image Restoration Tasks</strong>
    </a>
    <br/>
    Jiaxin Zhang, Dezhi Peng, Chongyu Liu, Peirong Zhang, Lianwen Jin
    <br/>
    [<a href="https://arxiv.org/abs/2405.04408">paper</a>] [<a href="https://github.com/ZZZHANG-jx/DocRes">code</a>]  [<a href="https://huggingface.co/spaces/qubvel-hf/documents-restoration">demo</a>] 
    <br/>
    <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>

### Efficient and scalable vision

- <p align="left">
    <a href="https://arxiv.org/abs/2312.00863" title="EfficientSAM: Leveraged Masked Image Pretraining for Efficient Segment Anything">
        <strong>🔥 EfficientSAM: Leveraged Masked Image Pretraining for Efficient Segment Anything</strong>
    </a>
    <br/>
    Yunyang Xiong, Bala Varadarajan, Lemeng Wu, Xiaoyu Xiang, Fanyi Xiao, Chenchen Zhu, Xiaoliang Dai, Dilin Wang, Fei Sun, Forrest Iandola, Raghuraman Krishnamoorthi, Vikas Chandra
    <br/>
    <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>


- <p align="left">
    <a href="https://arxiv.org/abs/2311.17049" title="MobileCLIP: Fast Image-Text Models through Multi-Modal Reinforced Training">
        <strong>MobileCLIP: Fast Image-Text Models through Multi-Modal Reinforced Training</strong>
    </a>
    <br/>
    Pavan Kumar Anasosalu Vasu, Hadi Pouransari, Fartash Faghri, Raviteja Vemulapalli, Oncel Tuzel
    <br/>
    <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>

### Explainable computer vision

- <p align="left">
    <a href="https://arxiv.org/abs/2312.02974" title="Describing Differences in Image Sets with Natural Language">
        <strong>🔥 Describing Differences in Image Sets with Natural Language</strong>
    </a>
    <br/>
    Lisa Dunlap, Yuhui Zhang, Xiaohan Wang, Ruiqi Zhong, Trevor Darrell, Jacob Steinhardt, Joseph E. Gonzalez, Serena Yeung-Levy
    <br/>
    [<a href="https://arxiv.org/abs/2312.02974">paper</a>] [<a href="https://github.com/Understanding-Visual-Datasets/VisDiff">code</a>]   
    <br/>
    <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>

### Low-level vision

- <p align="left">
    <a href="https://arxiv.org/abs/2404.19174" title="XFeat: Accelerated Features for Lightweight Image Matching">
        <strong>XFeat: Accelerated Features for Lightweight Image Matching</strong>
    </a>
    <br/>
    Guilherme Potje, Felipe Cadar, Andre Araujo, Renato Martins, Erickson R. Nascimento
    <br/>
    [<a href="https://arxiv.org/abs/2404.19174">paper</a>] [<a href="https://github.com/verlab/accelerated_features">code</a>] [<a href="https://youtu.be/RamC70IkZuI">video</a>] [<a href="https://huggingface.co/spaces/qubvel-hf/xfeat">demo</a>] [<a href="https://colab.research.google.com/github/verlab/accelerated_features/blob/main/notebooks/xfeat_matching.ipynb">colab</a>]
    <br/>
    <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>


- <p align="left">
    <a href="https://openaccess.thecvf.com/content/CVPR2024/html/Ryou_Robust_Image_Denoising_through_Adversarial_Frequency_Mixup_CVPR_2024_paper.html" title="Robust Image Denoising through Adversarial Frequency Mixup">
        <strong>Robust Image Denoising through Adversarial Frequency Mixup</strong>
    </a>
    <br/>
    Donghun Ryou, Inju Ha, Hyewon Yoo, Dongwan Kim, Bohyung Han
    <br/>
   <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>

### Multi-modal learning

- <p align="left">
    <a href="https://arxiv.org/abs/2310.03744" title="Improved Baselines with Visual Instruction Tuning">
        <strong>🔥 Improved Baselines with Visual Instruction Tuning</strong>
    </a>
    <br/>
    Haotian Liu, Chunyuan Li, Yuheng Li, Yong Jae Lee
    <br/>
  <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>

### Recognition: categorization, detection, retrieval

- <p align="left">
    <a href="https://arxiv.org/abs/2304.08069" title="DETRs Beat YOLOs on Real-time Object Detection">
        <strong>DETRs Beat YOLOs on Real-time Object Detection</strong>
    </a>
    <br/>
    Yian Zhao, Wenyu Lv, Shangliang Xu, Jinman Wei, Guanzhong Wang, Qingqing Dang, Yi Liu, Jie Chen
    <br/>
    <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>


- <p align="left">
    <a href="https://arxiv.org/abs/2401.17270" title="YOLO-World: Real-Time Open-Vocabulary Object Detection">
        <strong>YOLO-World: Real-Time Open-Vocabulary Object Detection</strong>
    </a>
    <br/>
    Tianheng Cheng, Lin Song, Yixiao Ge, Wenyu Liu, Xinggang Wang, Ying Shan
    <br/>
  <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>

<p align="left">
    <a href="https://arxiv.org/abs/2312.02142" title="Object Recognition as Next Token Prediction">
        <strong>🔥 Object Recognition as Next Token Prediction</strong>
    </a>
    <br/>
    Kaiyu Yue, Bor-Chun Chen, Jonas Geiping, Hengduo Li, Tom Goldstein, Ser-Nam Lim
    <br/>
    [<a href="https://arxiv.org/abs/2312.02142">paper</a>] [<a href="https://github.com/kaiyuyue/nxtp">code</a>] [<a href="https://youtu.be/xeI8dZIpoco">video</a>]  [<a href="https://colab.research.google.com/drive/1pJX37LP5xGLDzD3H7ztTmpq1RrIBeWX3?usp=sharing">colab</a>]
    <br/>
    <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>

### Segmentation, grouping and shape analysis

- <p align="left">
    <a href="https://openaccess.thecvf.com/content/CVPR2024/html/Chen_RobustSAM_Segment_Anything_Robustly_on_Degraded_Images_CVPR_2024_paper.html" title="RobustSAM: Segment Anything Robustly on Degraded Images">
        <strong>🔥 RobustSAM: Segment Anything Robustly on Degraded Images</strong>
    </a>
    <br/>
    Wei-Ting Chen, Yu-Jiet Vong, Sy-Yen Kuo, Sizhou Ma, Jian Wang
    <br/>
    <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>


- <p align="left">
    <a href="https://openaccess.thecvf.com/content/CVPR2024/html/Zhang_Frozen_CLIP_A_Strong_Backbone_for_Weakly_Supervised_Semantic_Segmentation_CVPR_2024_paper.html" title="Frozen CLIP: A Strong Backbone for Weakly Supervised Semantic Segmentation">
        <strong>🔥 Frozen CLIP: A Strong Backbone for Weakly Supervised Semantic Segmentation</strong>
    </a>
    <br/>
    Bingfeng Zhang, Siyue Yu, Yunchao Wei, Yao Zhao, Jimin Xiao
    <br/>
   <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>


- <p align="left">
    <a href="https://arxiv.org/abs/2312.15895" title="Semantic-aware SAM for Point-Prompted Instance Segmentation">
        <strong>🔥 Semantic-aware SAM for Point-Prompted Instance Segmentation</strong>
    </a>
    <br/>
    Zhaoyang Wei, Pengfei Chen, Xuehui Yu, Guorong Li, Jianbin Jiao, Zhenjun Han
    <br/>
    <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>


- <p align="left">
    <a href="https://arxiv.org/abs/2403.15789" title="In-Context Matting">
        <strong>In-Context Matting</strong>
    </a>
    <br/>
    He Guo, Zixuan Ye, Zhiguo Cao, Hao Lu
    <br/>
    <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>


- <p align="left">
    <a href="https://arxiv.org/abs/2312.09158" title="General Object Foundation Model for Images and Videos at Scale">
        <strong>General Object Foundation Model for Images and Videos at Scale</strong>
    </a>
    <br/>
    Junfeng Wu, Yi Jiang, Qihao Liu, Zehuan Yuan, Xiang Bai, Song Bai
    <br/>
     <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>

### Self-supervised or unsupervised representation learning

<p align="left">
    <a href="https://cvpr.thecvf.com/media/PosterPDFs/CVPR%202024/30014.png?t=1717339970.9614518" title="InternVL: Scaling up Vision Foundation Models and Aligning for Generic Visual-Linguistic Tasks">
        <img src="https://cvpr.thecvf.com/media/PosterPDFs/CVPR%202024/30014.png?t=1717339970.9614518" alt="InternVL: Scaling up Vision Foundation Models and Aligning for Generic Visual-Linguistic Tasks" width="400px" align="left" />
    </a>
    <a href="https://arxiv.org/abs/2312.14238" title="InternVL: Scaling up Vision Foundation Models and Aligning for Generic Visual-Linguistic Tasks">
        <strong>🔥 InternVL: Scaling up Vision Foundation Models and Aligning for Generic Visual-Linguistic Tasks</strong>
    </a>
    <br/>
    Zhe Chen, Jiannan Wu, Wenhai Wang, Weijie Su, Guo Chen, Sen Xing, Muyan Zhong, Qinglong Zhang, Xizhou Zhu, Lewei Lu, Bin Li, Ping Luo, Tong Lu, Yu Qiao, Jifeng Dai
    <br/>
    [<a href="https://arxiv.org/abs/2312.14238">paper</a>] [<a href="https://github.com/OpenGVLab/InternVL">code</a>]  [<a href="https://huggingface.co/spaces/OpenGVLab/InternVL">demo</a>] 
    <br/>
    <strong>Topic:</strong> Self-supervised or unsupervised representation learning
    <br/>
    <strong>Session:</strong> Fri 21 Jun 8 p.m. EDT — 9:30 p.m. EDT #412
</p>
<br/>
<br/>

### Video: low-level analysis, motion, and tracking

- <p align="left">
    <a href="https://arxiv.org/abs/2406.04221" title="Matching Anything by Segmenting Anything">
        <strong>🔥 Matching Anything by Segmenting Anything</strong>
    </a>
    <br/>
    Siyuan Li, Lei Ke, Martin Danelljan, Luigi Piccinelli, Mattia Segu, Luc Van Gool, Fisher Yu
    <br/>
  <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>

- <p align="left">
    <a href="https://arxiv.org/abs/2403.02075" title="DiffMOT: A Real-time Diffusion-based Multiple Object Tracker with Non-linear Prediction">
        <strong>DiffMOT: A Real-time Diffusion-based Multiple Object Tracker with Non-linear Prediction</strong>
    </a>
    <br/>
    Weiyi Lv, Yuhang Huang, Ning Zhang, Ruei-Sung Lin, Mei Han, Dan Zeng
    <br/>
     <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>

### Vision, language, and reasoning

- <p align="left">
    <a href="https://arxiv.org/abs/2312.03818" title="Alpha-CLIP: A CLIP Model Focusing on Wherever You Want">
        <strong>Alpha-CLIP: A CLIP Model Focusing on Wherever You Want</strong>
    </a>
    <br/>
    Zeyi Sun, Ye Fang, Tong Wu, Pan Zhang, Yuhang Zang, Shu Kong, Yuanjun Xiong, Dahua Lin, Jiaqi Wang
    <br/>
    <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>


- <p align="left">
    <a href="https://arxiv.org/abs/2401.06209" title="Eyes Wide Shut? Exploring the Visual Shortcomings of Multimodal LLMs">
        <strong>🔥 Eyes Wide Shut? Exploring the Visual Shortcomings of Multimodal LLMs</strong>
    </a>
    <br/>
    Shengbang Tong, Zhuang Liu, Yuexiang Zhai, Yi Ma, Yann LeCun, Saining Xie
    <br/>
     <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>


- <p align="left">
    <a href="https://arxiv.org/abs/2308.00692" title="LISA: Reasoning Segmentation via Large Language Model">
        <strong>🔥 LISA: Reasoning Segmentation via Large Language Model</strong>
    </a>
    <br/>
    Xin Lai, Zhuotao Tian, Yukang Chen, Yanwei Li, Yuhui Yuan, Shu Liu, Jiaya Jia
    <br/>
   <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>


- <p align="left">
    <a href="https://arxiv.org/abs/2312.00784" title="ViP-LLaVA: Making Large Multimodal Models Understand Arbitrary Visual Prompts">
        <strong>ViP-LLaVA: Making Large Multimodal Models Understand Arbitrary Visual Prompts</strong>
    </a>
    <br/>
    Mu Cai, Haotian Liu, Dennis Park, Siva Karthik Mustikovela, Gregory P. Meyer, Yuning Chai, Yong Jae Lee
    <br/>
  <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>


- <p align="left">
    <a href="https://arxiv.org/abs/2311.16502" title="MMMU: A Massive Multi-discipline Multimodal Understanding and Reasoning Benchmark for Expert AGI">
        <strong>🔥 MMMU: A Massive Multi-discipline Multimodal Understanding and Reasoning Benchmark for Expert AGI</strong>
    </a>
    <br/>
    Xiang Yue, Yuansheng Ni, Kai Zhang, Tianyu Zheng, Ruoqi Liu, Ge Zhang, Samuel Stevens, Dongfu Jiang, Weiming Ren, Yuxuan Sun, Cong Wei, Botao Yu, Ruibin Yuan, Renliang Sun, Ming Yin, Boyuan Zheng, Zhenzhu Yang, Yibo Liu, Wenhao Huang, Huan Sun, Yu Su, Wenhu Chen
    <br/>
     <a href="https://arxiv.org/pdf/2311.06242"><img src="https://img.shields.io/badge/arXiv-Florence2-b31b1b.svg" height=20.5></a> 
    <a href="https://openaccess.thecvf.com/content/CVPR2024/papers/Xiao_Florence-2_Advancing_a_Unified_Representation_for_a_Variety_of_Vision_CVPR_2024_paper.pdf"><img src="https://img.shields.io/badge/Download%20as%20PDF-EF3939?style=flat&logo=adobeacrobatreader&logoColor=white&color=black&labelColor=ec1c24" height=20.5></a> <a href=""><img src="https://img.shields.io/badge/github-%23121011.svg?style=for-the-badge&logo=github&logoColor=white", height=20.5></a> <a href="https://delinqu.github.io/EN-SLAM/"><img src="https://img.shields.io/badge/Project_Page-ENSLAM-blue' alt='Project Page"></a> <a href="https://youtu.be/cOlyA00K1ec"><img src="https://img.shields.io/static/v1?label=Youtube&message=Link&color=red" height=20.5></a> 
    <br/>
    <strong>Likely application in agriculture:</strong> Agricultural robot localization
</p>

<!--- AUTOGENERATED_PAPERS_LIST -->

## 🦸 contribution

We would love your help in making this repository even better! If you know of an amazing
paper that isn't listed here, or if you have any suggestions for improvement, feel free
to open an
[issue](https://github.com/SkalskiP/top-cvpr-2024-papers/issues)
or submit a
[pull request](https://github.com/SkalskiP/top-cvpr-2024-papers/pulls).
