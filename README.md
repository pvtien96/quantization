# Quantization
[![Awesome](https://cdn.rawgit.com/sindresorhus/awesome/d7305f38d29fed78fa85652e3a63e154dd8e8829/media/badge.svg)](https://github.com/sindresorhus/awesome)
![GitHub last commit](https://img.shields.io/github/last-commit/pvtien96/quantization)
![Visitors](https://api.visitorbadge.io/api/combined?path=https%3A%2F%2Fgithub.com%2Fpvtien96%2Fquantization&label=visitors&countColor=%23263759&style=flat)

## :books: Surveys
<details>
<summary><a href="https://arxiv.org/pdf/2312.03863.pdf" target="_blank"><strong>Efficient Large Language Models: A Survey</strong></a></summary>

- **Abstract:** Large Language Models (LLMs) have demonstrated remarkable capabilities in important tasks such as natural language understanding, language generation, and complex reasoning and have the potential to make a substantial impact on our society. Such capabilities, however, come with the considerable resources they demand, highlighting the strong need to develop effective techniques for addressing their efficiency challenges. In this survey, we provide a systematic and comprehensive review of efficient LLMs research. We organize the literature in a taxonomy consisting of three main categories, covering distinct yet interconnected efficient LLMs topics from model-centric, data-centric, and framework-centric perspective, respectively. We have also created a GitHub repository where we compile the papers featured in this survey at this https URL, this https URL, and will actively maintain this repository and incorporate new research as it emerges. We hope our survey can serve as a valuable resource to help researchers and practitioners gain a systematic understanding of the research developments in efficient LLMs and inspire them to contribute to this important and exciting field.
- **Comments:**

</details>

<details>
<summary><a href="https://arxiv.org/abs/2308.07633" target="_blank"><strong>A Survey on Model Compression for Large Language Models</strong></a></summary>

- **Abstract:** Large Language Models (LLMs) have revolutionized natural language processing tasks with remarkable success. However, their formidable size and computational demands present significant challenges for practical deployment, especially in resource-constrained environments. As these challenges become increasingly pertinent, the field of model compression has emerged as a pivotal research area to alleviate these limitations. This paper presents a comprehensive survey that navigates the landscape of model compression techniques tailored specifically for LLMs. Addressing the imperative need for efficient deployment, we delve into various methodologies, encompassing quantization, pruning, knowledge distillation, and more. Within each of these techniques, we highlight recent advancements and innovative approaches that contribute to the evolving landscape of LLM research. Furthermore, we explore benchmarking strategies and evaluation metrics that are essential for assessing the effectiveness of compressed LLMs. By providing insights into the latest developments and practical implications, this survey serves as an invaluable resource for both researchers and practitioners. As LLMs continue to evolve, this survey aims to facilitate enhanced efficiency and real-world applicability, establishing a foundation for future advancements in the field.
- **Comments:**

</details>

<details>
<summary><a href="https://arxiv.org/abs/2103.13630" target="_blank"><strong>A Survey of Quantization Methods for Efficient Neural Network Inference</strong></a></summary>

- **Abstract:** As soon as abstract mathematical computations were adapted to computation on digital computers, the problem of efficient representation, manipulation, and communication of the numerical values in those computations arose. Strongly related to the problem of numerical representation is the problem of quantization: in what manner should a set of continuous real-valued numbers be distributed over a fixed discrete set of numbers to minimize the number of bits required and also to maximize the accuracy of the attendant computations? This perennial problem of quantization is particularly relevant whenever memory and/or computational resources are severely restricted, and it has come to the forefront in recent years due to the remarkable performance of Neural Network models in computer vision, natural language processing, and related areas. Moving from floating-point representations to low-precision fixed integer values represented in four bits or less holds the potential to reduce the memory footprint and latency by a factor of 16x; and, in fact, reductions of 4x to 8x are often realized in practice in these applications. Thus, it is not surprising that quantization has emerged recently as an important and very active sub-area of research in the efficient implementation of computations associated with Neural Networks. In this article, we survey approaches to the problem of quantizing the numerical values in deep Neural Network computations, covering the advantages/disadvantages of current methods. With this survey and its organization, we hope to have presented a useful snapshot of the current research in quantization for Neural Networks and to have given an intelligent organization to ease the evaluation of future research in this area.
- **Comments:**

</details>


## :clipboard: Research Papers
<details>
<summary><a href="https://arxiv.org/abs/2309.05516" target="_blank"><strong>10. Optimize Weight Rounding via Signed Gradient Descent for the Quantization of LLMs</strong></a></summary>

- **TLDR:**
- **Abstract:** Large Language Models (LLMs) have proven their exceptional capabilities in performing language-related tasks. However, their deployment poses significant challenges due to their considerable memory and storage requirements. In response to this issue, weight-only quantization, particularly 3 and 4-bit weight-only quantization, has emerged as one of the most viable solutions. As the number of bits decreases, the quantization grid broadens, thus emphasizing the importance of up and down rounding. While previous studies have demonstrated that fine-tuning up and down rounding with the addition of perturbations can enhance accuracy in some scenarios, our study is driven by the precise and limited boundary of these perturbations, where only the threshold for altering the rounding value is of significance. Consequently, we propose a concise and highly effective approach for optimizing the weight rounding task. Our method, named SignRound, involves lightweight block-wise tuning using signed gradient descent, enabling us to achieve outstanding results within 400 steps. SignRound competes impressively against recent methods without introducing additional inference overhead.
- **What:**
- **Methodology:**
- **Conclusions:**
- **Limitations:**
- **Comments:**: Contaning a comprehensive comparison.

</details>
<details>
<summary><a href="https://arxiv.org/abs/2210.17323" target="_blank"><strong>9. GPTQ: Accurate Post-Training Quantization for Generative Pre-trained Transformers</strong></a></summary>

- **TLDR:**
- **Abstract:** Generative Pre-trained Transformer models, known as GPT or OPT, set themselves apart through breakthrough performance across complex language modelling tasks, but also by their extremely high computational and storage costs. Specifically, due to their massive size, even inference for large, highly-accurate GPT models may require multiple performant GPUs, which limits the usability of such models. While there is emerging work on relieving this pressure via model compression, the applicability and performance of existing compression techniques is limited by the scale and complexity of GPT models. In this paper, we address this challenge, and propose GPTQ, a new one-shot weight quantization method based on approximate second-order information, that is both highly-accurate and highly-efficient. Specifically, GPTQ can quantize GPT models with 175 billion parameters in approximately four GPU hours, reducing the bitwidth down to 3 or 4 bits per weight, with negligible accuracy degradation relative to the uncompressed baseline. Our method more than doubles the compression gains relative to previously-proposed one-shot quantization methods, preserving accuracy, allowing us for the first time to execute an 175 billion-parameter model inside a single GPU for generative inference. Moreover, we also show that our method can still provide reasonable accuracy in the extreme quantization regime, in which weights are quantized to 2-bit or even ternary quantization levels. We show experimentally that these improvements can be leveraged for end-to-end inference speedups over FP16, of around 3.25x when using high-end GPUs (NVIDIA A100) and 4.5x when using more cost-effective ones (NVIDIA A6000). The implementation is available at this https URL.
- **What:**
- **Methodology:**
- **Conclusions:**
- **Limitations:**
- **Comments:**: Foundation.

</details>

<details>
<summary><a href="https://arxiv.org/abs/2402.15319" target="_blank"><strong>8. GPTVQ: The Blessing of Dimensionality for LLM Quantization</strong></a></summary>

- **TLDR:**
- **Abstract:** In this work we show that the size versus accuracy trade-off of neural network quantization can be significantly improved by increasing the quantization dimensionality. We propose the GPTVQ method, a new fast method for post-training vector quantization (VQ) that scales well to Large Language Models (LLMs). Our method interleaves quantization of one or more columns with updates to the remaining unquantized weights, using information from the Hessian of the per-layer output reconstruction MSE. Quantization codebooks are initialized using an efficient data-aware version of the EM algorithm. The codebooks are then updated, and further compressed by using integer quantization and SVD-based compression. GPTVQ establishes a new state-of-the art in the size vs accuracy trade-offs on a wide range of LLMs such as Llama-v2 and Mistral. Furthermore, our method is efficient: on a single H100 it takes between 3 and 11 hours to process a Llamav2-70B model, depending on quantization setting. Lastly, with on-device timings for VQ decompression on a mobile CPU we show that VQ leads to improved latency compared to using a 4-bit integer format.
- **What:**
- **Methodology:**
- **Conclusions:**
- **Limitations:**
- **Comments:**: SVD.

</details>


<details>
<summary><a href="https://arxiv.org/abs/2310.08659" target="_blank"><strong>7. LoftQ: LoRA-Fine-Tuning-Aware Quantization for Large Language Models </strong></a></summary> 
  

- **TLDR:** LoftQ finds good enough quantized LoRA initialization: quantized backbone Q and LoRA adapters A and B, given a pre-trained weight W.
- **Abstract:** Quantization is an indispensable technique for serving Large Language Models (LLMs) and has recently found its way into LoRA fine-tuning. In this work we focus on the scenario where quantization and LoRA fine-tuning are applied together on a pre-trained model. In such cases it is common to observe a consistent gap in the performance on downstream tasks between full fine-tuning and quantization plus LoRA fine-tuning approach. In response, we propose LoftQ (LoRA-Fine-Tuning-aware Quantization), a novel quantization framework that simultaneously quantizes an LLM and finds a proper low-rank initialization for LoRA fine-tuning. Such an initialization alleviates the discrepancy between the quantized and full-precision model and significantly improves generalization in downstream tasks. We evaluate our method on natural language understanding, question answering, summarization, and natural language generation tasks. Experiments show that our method is highly effective and outperforms existing quantization methods, especially in the challenging 2-bit and 2/4-bit mixed precision regimes.
- [![GitHub Repo stars](https://img.shields.io/github/stars/yxli2123/LoftQ)](https://github.com/yxli2123/LoftQ)
</details>

<details>
<summary><a href="https://arxiv.org/abs/2311.12023" target="_blank"><strong>1. LQ-LoRA: Low-rank Plus Quantized Matrix Decomposition for Efficient Language Model Finetuning</strong></a></summary>

- **TLDR:** Decompose a matrix into low-rank component and a memory-efficient quantized component.
- **Abstract:** We propose a simple approach for memory-efficient adaptation of pretrained language models. Our approach uses an iterative algorithm to decompose each pretrained matrix into a high-precision low-rank component and a memory-efficient quantized component. During finetuning, the quantized component remains fixed and only the low-rank component is updated. We present an integer linear programming formulation of the quantization component which enables dynamic configuration of quantization parameters (e.g., bit-width, block size) for each matrix given an overall target memory budget. We further explore a data-aware version of the algorithm which uses an approximation of the Fisher information matrix to weight the reconstruction objective during matrix decomposition. Experiments on adapting RoBERTa and LLaMA-2 (7B and 70B) demonstrate that our low-rank plus quantized matrix decomposition approach (LQ-LoRA) outperforms strong QLoRA and GPTQ-LoRA baselines and moreover enables more aggressive quantization. For example, on the OpenAssistant benchmark LQ-LoRA is able to learn a 2.5-bit LLaMA-2 model that is competitive with a model finetuned with 4-bit QLoRA. When finetuned on a language modeling calibration dataset, LQ-LoRA can also be used for model compression; in this setting our 2.75-bit LLaMA-2-70B model (which has 2.85 bits on average when including the low-rank components and requires 27GB of GPU memory) is competitive with the original model in full precision.
- **What:**
- **Methodology:**
- **Conclusions:**
- **Limitations:**
- **Comments:** First paper.

</details>

<details>
<summary><a href="https://arxiv.org/abs/2306.00978" target="_blank"><strong>2. AWQ: Activation-aware Weight Quantization for LLM Compression and Acceleration</strong></a></summary>

- **TLDR:** .
- **Abstract:** Large language models (LLMs) have shown excellent performance on various tasks, but the astronomical model size raises the hardware barrier for serving (memory size) and slows down token generation (memory bandwidth). In this paper, we propose Activation-aware Weight Quantization (AWQ), a hardware-friendly approach for LLM low-bit weight-only quantization. Our method is based on the observation that weights are not equally important: protecting only 1% of salient weights can greatly reduce quantization error. We then propose to search for the optimal per-channel scaling that protects the salient weights by observing the activation, not weights. AWQ does not rely on any backpropagation or reconstruction, so it can well preserve LLMs' generalization ability on different domains and modalities, without overfitting to the calibration set. AWQ outperforms existing work on various language modeling and domain-specific benchmarks. Thanks to better generalization, it achieves excellent quantization performance for instruction-tuned LMs and, for the first time, multi-modal LMs. Alongside AWQ, we implement an efficient and flexible inference framework tailored for LLMs on the edge, offering more than 3x speedup over the Huggingface FP16 implementation on both desktop and mobile GPUs. It also democratizes the deployment of the 70B Llama-2 model on mobile GPU (NVIDIA Jetson Orin 64GB).
- **What:**
  - LLMs's large size leads to high cost.
  - Quantization-aware training (QAT): high training cost. Post-training quantization (PTQ) suffers from large accuracy degradation under a low-bit setting. GPTQ distorts the learned features on out-of-distribution domains.
- **Observation:**
  - Weights are not equally important. Weight channels corresponding to larger activation magnitudes are more salient since they process more important features.
    ![image](https://github.com/pvtien96/quantization/assets/25927039/c81d7f97-c4ef-4540-ab52-74e04c16ada5)
  - Selecting weights based on activation magnitude can significantly improve the performance: keeping only 0.1%-1% of the channels corresponding to larger activation significantly improves the quantized performance.
  - Such a mixed-precision data type will make the system implementation difficult.

- **Methodology:**
  - To avoid the hardware-inefficient mixed-precision implementation: scaling up the salient channels can reduce their relative quantization error.
  ![image](https://github.com/pvtien96/quantization/assets/25927039/f27b3bc8-ebf6-42d9-8780-61cc03895f3d)
  - To consider both salient and non-salient weights: automatically search for an optimal (per input channel) scaling factor that minimizes the output difference after quantization for a certain layer.
  ![image](https://github.com/pvtien96/quantization/assets/25927039/46fef7f8-d256-4e6e-8cbe-dee1dc6d47cc)
- **Conclusions:**
- **Limitations:**
- **Comments:**
  - Why $0.1\%$ salaient weights? How to define the portion of salient weight? Should we make it adaptive  (*e.g.,* per layer)
  - How do we select salient channels? Anything else better than activation distribution?
  - Any optimization techniques without mixed precision
  - **Decompose (*e.g.,* SVD, which (weight, activation, gradient), in which data form) then quantize factor matrices.**

</details>

<details>
<summary><a href="https://www.youtube.com/watch?v=MK4k64vY3xo&ab_channel=MITHANLab" target="_blank"><strong>3. EfficientML.ai Lecture 5 - Quantization</strong></a></summary>

- **TLDR:** fundamental.
- **Definitions:**
    - Quantization is the process of constraining an input from a continuous or otherwise large set of values (such as the real numbers) to a discrete set (such as the integers).
    - The difference between an input value and its quantized value
    is referred to as quantization error.
    <p align="center" width="100%">
    <img src="assets\quantization error.png" width="40%" height="50%">
    </p>
- **Categorization:**
    - K-Means-Based Quantization: apply quantization-aware training.
    - Linear Quantization: apply integer-only inference.
    <p align="center" width="100%">
    <img src="assets\kmeans_vs_linear_quantization.png" width="40%" height="50%">
    </p>
- **Comments:**
    - Notebook: https://colab.research.google.com/drive/1z0D3pBb3uy3VvK0Lu01d5C_Sq1j7d-rt?usp=sharing
    - Solution: https://github.com/yifanlu0227/MIT-6.5940/tree/main

</details>

<details>
<summary><a href="https://arxiv.org/abs/1712.05877" target="_blank"><strong>4. Quantization and Training of Neural Networks for Efficient Integer-Arithmetic-Only Inference</strong></a></summary>

- **TLDR:** .
- **Abstract:** The rising popularity of intelligent mobile devices and the daunting computational cost of deep learning-based models call for efficient and accurate on-device inference schemes. We propose a quantization scheme that allows inference to be carried out using integer-only arithmetic, which can be implemented more efficiently than floating point inference on commonly available integer-only hardware. We also co-design a training procedure to preserve end-to-end model accuracy post quantization. As a result, the proposed quantization scheme improves the tradeoff between accuracy and on-device latency. The improvements are significant even on MobileNets, a model family known for run-time efficiency, and are demonstrated in ImageNet classification and COCO detection on popular CPUs.
- **What:** an affine mapping of integers $q$ to real numbers $r$, expressed as $r = S(q − Z)$ where $S$ is scaling and $Z$ is zero-point parameter.
- **Methodology:** Integer-arithmetic-only quantization, including: integer-arithmetic-only inference, simulated quantization training.
- **Conclusions:**
- **Limitations:**
- **Comments:**

</details>

<details>
<summary><a href="https://arxiv.org/abs/1510.00149" target="_blank"><strong>5. Deep Compression: Compressing Deep Neural Networks with Pruning, Trained Quantization and Huffman Coding</strong></a></summary>

- **TLDR:**
- **Abstract:** Neural networks are both computationally intensive and memory intensive, making them difficult to deploy on embedded systems with limited hardware resources. To address this limitation, we introduce "deep compression", a three stage pipeline: pruning, trained quantization and Huffman coding, that work together to reduce the storage requirement of neural networks by 35x to 49x without affecting their accuracy. Our method first prunes the network by learning only the important connections. Next, we quantize the weights to enforce weight sharing, finally, we apply Huffman coding. After the first two steps we retrain the network to fine tune the remaining connections and the quantized centroids. Pruning, reduces the number of connections by 9x to 13x; Quantization then reduces the number of bits that represent each connection from 32 to 5. On the ImageNet dataset, our method reduced the storage required by AlexNet by 35x, from 240MB to 6.9MB, without loss of accuracy. Our method reduced the size of VGG-16 by 49x from 552MB to 11.3MB, again with no loss of accuracy. This allows fitting the model into on-chip SRAM cache rather than off-chip DRAM memory. Our compression method also facilitates the use of complex neural networks in mobile applications where application size and download bandwidth are constrained. Benchmarked on CPU, GPU and mobile GPU, compressed network has 3x to 4x layerwise speedup and 3x to 7x better energy efficiency.
- **What:**
- **Methodology:**
  <p align="center" width="100%">
    <img src="assets\deep_compression.png" width="80%" height="50%">
  </p>
  <p align="center" width="100%">
    <img src="assets\kmeans_quantization.png" width="80%" height="50%">
  </p>
- **Conclusions:**
  <p align="center" width="100%">
    <img src="assets\accuracy_vs_compression.png" width="80%" height="50%">
  </p>
- **Limitations:**
  - only save storage, doesn't accelerate training/inference speed
  - complicated implementation
- **Comments:** hybrid compression.

</details>

<details>
<summary><a href="https://arxiv.org/abs/2106.09685" target="_blank"><strong>6. LoRA: Low-Rank Adaptation of Large Language Models</strong></a></summary>

- **TLDR:**
- **Abstract:** An important paradigm of natural language processing consists of large-scale pre-training on general domain data and adaptation to particular tasks or domains. As we pre-train larger models, full fine-tuning, which retrains all model parameters, becomes less feasible. Using GPT-3 175B as an example -- deploying independent instances of fine-tuned models, each with 175B parameters, is prohibitively expensive. We propose Low-Rank Adaptation, or LoRA, which freezes the pre-trained model weights and injects trainable rank decomposition matrices into each layer of the Transformer architecture, greatly reducing the number of trainable parameters for downstream tasks. Compared to GPT-3 175B fine-tuned with Adam, LoRA can reduce the number of trainable parameters by 10,000 times and the GPU memory requirement by 3 times. LoRA performs on-par or better than fine-tuning in model quality on RoBERTa, DeBERTa, GPT-2, and GPT-3, despite having fewer trainable parameters, a higher training throughput, and, unlike adapters, no additional inference latency. We also provide an empirical investigation into rank-deficiency in language model adaptation, which sheds light on the efficacy of LoRA. We release a package that facilitates the integration of LoRA with PyTorch models and provide our implementations and model checkpoints for RoBERTa, DeBERTa, and GPT-2.
- **What:**
- **Methodology:**
- **Conclusions:**
- **Limitations:**
- **Comments:**: foundation paper.

</details>


## :computer: Repositories
- https://github.com/Zhen-Dong/Awesome-Quantization-Papers
- https://github.com/htqin/awesome-model-quantization
- https://github.com/AIoT-MLSys-Lab/Efficient-LLMs-Survey
- https://github.com/HuangOwen/Awesome-LLM-Compression
- https://github.com/intel/neural-compressor/blob/master/docs/source/quantization.md
- https://github.com/AutoGPTQ/AutoGPTQ
- https://github.com/IST-DASLab
