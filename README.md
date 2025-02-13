# RAGCap: Retrieval-Augmented Generation for Remote Sensing Image Captioning

 Yakoub Bazi, Mohamad M. Al Rahhal, Mansour Zuair
[[Paper]()] [[RAGCap]] [[Dataset]] 


<br>

## Content 📒
-
- [Abstract](#Abstract)
- [Architecture](#Architecture)
- [Results](#Results)
- [Citation](#citation)

---
## Abstract
Remote Sensing (RS) image captioning has traditionally relied on specialized models tailored to domain-specific tasks. The emergence of large vision-language models (VLMs) offers a promising alternative due to their versatility across tasks and domains. However, fine-tuning VLMs for specific applications introduces significant challenges, including computational overhead, overfitting risks, and reduced generalization capabilities. To address these limitations, we propose RAGCap a Retrieval-Augmented Generation framework that leverages pre-trained VLMs for RS captioning without the need for fine-tuning. Our approach employs a similarity-based retrieval model (SigLIP) to identify relevant image-caption pairs from the training set. These retrieved examples, along with the test image, are processed by a multi-image capable VLM (Qwen2VL) using a carefully designed prompt structure. This enables the model to generate captions that not only accurately describe the test image but also preserve the domain-specific style. Extensive evaluations on three RS benchmark datasets demonstrate that RAGCap achieves competitive performance compared to fine-tuned models while offering enhanced efficiency and generalization. Our framework provides a practical and scalable solution, maintaining the versatility of VLMs while effectively adapting to domain-specific requirements

## Architecture
<p align="center">
  <img width="600" src="https://github.com/BigData-KSU/RAGCap/blob/main/methodology_graph..png" alt="RAGCap Architectural Overview">
</p>

## Results
<p align="center">
  <img width="600" src="https://github.com/BigData-KSU/RAGCap/blob/main/Results_Table.png" alt="Results Table">
</p>

<p align="center">
  <img width="600" src="https://github.com/BigData-KSU/RAGCap/blob/main/Results_Graph.png" alt="Results Graph">
</p>

## Citation
Coming soon
