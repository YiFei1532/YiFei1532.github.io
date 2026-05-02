---
permalink: /
title: ""
excerpt: ""
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<span class='anchor' id='about-me'></span>

Hi! I'm Yifei Xia, a second-year Ph.D. student in the [School of Computer Science](https://cs.pku.edu.cn/) at [Peking University](https://www.pku.edu.cn/) and a member of [DAIR Lab](https://pkudair.github.io/), advised by Prof. [Bin Cui](https://cuibinpku.github.io/). I received my B.Sc. degree in Computer Science and Technology from the Turing Experimental Class at [Renmin University of China](https://www.ruc.edu.cn/) in June 2024, where I was advised by Prof. [Feng Zhang](https://fengzhangcs.github.io/).

I am the creator of [HetuDiT](https://github.com/PKU-DAIR/Hetu-DiT), an efficient and dynamic serving system for image and video generation models, and a developer of [Hetu](https://github.com/PKU-DAIR/Hetu), a high-performance distributed deep learning system for large-scale and automated parallel training, including LLM training workloads.

My research interests lie in **AI infrastructure**, especially **DiT post-train, inference and serving**, **LLM inference and serving**, and multi-modal training/inference systems.

**I am open to collaborations and discussions on efficient inference, serving systems, and AI infrastructure. Feel free to reach out!**

# 📖 Educations

* B.S. in Computer Science and Technology, Turing Experimental Class, Renmin University of China. 2020 - 2024. Adviser: [Feng Zhang](https://fengzhangcs.github.io/)

* Ph.D. in Computer Science and Technology, Peking University. 2024 - present. Adviser: [Bin Cui](https://cuibinpku.github.io/)

# 📝 Publications

## 2026

- **[ICML]** **Yifei Xia**, Fangcheng Fu, Hao Yuan, Bin Cui, et al. "EchoAttention: Exploiting Token-Pair Redundancy and Frame-Block Similarity for Efficient Long Video Generation." (coming soon)

## 2025

- **[arXiv]** **Yifei Xia**, Fangcheng Fu, Hao Yuan, Hanke Zhang, Xupeng Miao, Yijun Liu, Suhan Ling, Jie Jiang, Bin Cui. ["TridentServe: A Stage-level Serving System for Diffusion Pipelines."](https://arxiv.org/abs/2510.02838)

- **[ICCV]** **Yifei Xia**, Suhan Ling, Fangcheng Fu, Bin Cui, et al. ["Training-free and Adaptive Sparse Attention for Efficient Long Video Generation."](https://openaccess.thecvf.com/content/ICCV2025/html/Xia_Training-free_and_Adaptive_Sparse_Attention_for_Efficient_Long_Video_Generation_ICCV_2025_paper.html)

- **[KDD]** Zheng Chen, Feng Zhang, **Yifei Xia**, Wentao Zhang, Xiaowei Zhu, Wenguang Chen, Xiaoyong Du. ["CompressGNN: Accelerating Graph Neural Network Training via Hierarchical Compression."](https://doi.org/10.1145/3711896.3736888)

## 2024

- **[NeurIPS]** **Yifei Xia**, Fangcheng Fu, Wentao Zhang, Jiawei Jiang, Bin Cui. ["Efficient Multi-task LLM Quantization and Serving for Multiple LoRA Adapters."](https://proceedings.neurips.cc/paper_files/paper/2024/hash/747dc7c6566c74eb9a663bcd8d057c78-Abstract-Conference.html)

- **[VLDBJ]** **Yifei Xia**, Feng Zhang, Qingyu Xu, Mingde Zhang, Bingsheng He, et al. ["GPU-Based Butterfly Counting."](https://doi.org/10.1007/s00778-024-00861-0)

## 2023

- **[TPDS]** Yihua Hu, Feng Zhang, **Yifei Xia**, Zhiming Yao, Letian Zeng, Haipeng Ding, Zhewei Wei, Xiao Zhang, Jidong Zhai, Xiaoyong Du, Siqi Ma. ["Enabling Efficient Random Access to Hierarchically Compressed Text Data on Diverse GPU Platforms."](https://siqima.me/publications/GPU.pdf)

# 🚀 Systems

<div style="display: flex; gap: 20px; border: 1px solid #e0e0e0; border-radius: 8px; padding: 20px; margin-bottom: 20px; box-shadow: 0 2px 4px rgba(0,0,0,0.1);">
  <div style="width: 200px; flex-shrink: 0; display: flex; flex-direction: column; align-items: center;">
    <img src='images/hetudit-logo.png' alt="HetuDiT" style="width: 100%; max-width: 200px;">
  </div>
  <div style="flex: 1; min-width: 0;">
    <h3 style="margin-top: 0;"><a href="https://github.com/PKU-DAIR/Hetu-DiT">HetuDiT</a> - A Dynamic Serving System for Diffusion Transformers</h3>
    <p><strong>Creator</strong> | <a href="https://github.com/PKU-DAIR/Hetu-DiT"><strong>GitHub</strong></a> | <a href="https://arxiv.org/abs/2510.02838"><strong>Paper</strong></a></p>
    <p>HetuDiT is a stage-level, dynamically parallel serving system for Diffusion Transformers (DiTs). It targets real-world image and video generation serving workloads where requests differ in prompt length, resolution, frame count, and stage-level compute demand.</p>
    <ul>
      <li><strong>Stage-level scheduling</strong>: Profiles condition encoding, denoising, VAE decoding, and other stages separately, then rewrites execution plans on the fly.</li>
      <li><strong>Dynamic parallelism</strong>: Assigns stage-specific batch sizes and parallelism strategies, including SP, CP, TP, and PP, for each request stage.</li>
      <li><strong>Model support</strong>: Provides serving scripts for Stable Diffusion 3, CogVideoX 1.5-5B, Flux, and HunyuanVideo.</li>
      <li><strong>Serving performance</strong>: README benchmarks report higher SLO attainment and lower mean/P95 latency than static pipeline-level serving on a 128x NVIDIA L20 cluster.</li>
    </ul>
  </div>
</div>

<div style="display: flex; gap: 20px; border: 1px solid #e0e0e0; border-radius: 8px; padding: 20px; margin-bottom: 20px; box-shadow: 0 2px 4px rgba(0,0,0,0.1);">
  <div style="width: 200px; flex-shrink: 0; display: flex; flex-direction: column; align-items: center;">
    <img src='images/hetu-logo.png' alt="Hetu" style="width: 100%; max-width: 200px;">
  </div>
  <div style="flex: 1; min-width: 0;">
    <h3 style="margin-top: 0;"><a href="https://github.com/PKU-DAIR/Hetu">Hetu</a> - A Distributed Deep Learning System</h3>
    <p><strong>Developer</strong> | <a href="https://github.com/PKU-DAIR/Hetu"><strong>GitHub</strong></a> | <a href="https://hetu-doc.readthedocs.io"><strong>Documentation</strong></a></p>
    <p>Hetu is a high-performance distributed deep learning system developed by DAIR Lab at Peking University. It targets large-scale and automated distributed training, including trillion-parameter model training and modern LLM-related workloads.</p>
    <ul>
      <li><strong>Parallel training</strong>: Supports multiple training protocols and communication architectures, including data/model/pipeline parallelism, parameter server, and AllReduce.</li>
      <li><strong>Large-scale workloads</strong>: Designed for giant models and large-scale training workloads across distributed GPU clusters.</li>
      <li><strong>Research coverage</strong>: Serves as a platform for system research across Transformer/LLM, MoE, embedding, diffusion, GNN, heterogeneous-resource, kernel, and memory-management workloads.</li>
      <li><strong>Open ecosystem</strong>: Provides documentation, examples, and an Apache-2.0 open-source codebase maintained under PKU-DAIR.</li>
    </ul>
  </div>
</div>

# 🎖 Honors and Awards

* **Peking University Presidential Scholarship, 2025** (**top 1.5%, highest honor for Ph.D. students at Peking University**)

* **Peking University Presidential Scholarship, 2024** (**top 1.5%, highest honor for Ph.D. students at Peking University**)

* **China Institute of Electronics - Tencent Ph.D. Research Incentive Program**, Hunyuan Foundation Model Special Track, 2024 (**100,000 RMB, only 17 recipients nationwide**)

* **Best Paper** Award at CCF National Database Conference NDBC, 2024

* Outstanding Graduate, Renmin University of China, 2024

* Outstanding Undergraduate Thesis, Renmin University of China, 2024

* PetroChina Scholarship, 2023

* **National Scholarship, 2022** (**top 1%**)

* RUC-Huawei "Intelligent Base" Student Scholarship, 2022 and 2023

# 💻 Internships

- **[2024.09 - present]** Research Intern, Seed CV-AI Platform, ByteDance.

<div style="width: 50%;">
  <script type="text/javascript" id="mapmyvisitors" src="//mapmyvisitors.com/map.js?d=JeaFjgFKbmu2Be_TMFmkDwDlgmfcXbwd0kq4eThvKPg&cl=ffffff&w=a"></script>
</div>
