# RAGCap: Retrieval-Augmented Generation for Remote Sensing Image Captioning

 Yakoub Bazi, Mohamad M. Al Rahhal, Mansour Zuair
 
[[Paper]()] [[RAGCap]] [[Dataset]] 


<br>

## Content 📒
- [Abstract](#Abstract)
- [Architecture](#Architecture)
- [Results](#Results)
- [Citation](#citation)

<p>
  <a href="https://www.techrxiv.org/users/879731/articles/1274474-ragcap-retrieval-augmented-generation-for-style-aware-remote-sensing-image-captioning-without-fine-tuning?commit=2ba368c4b9de06be4576e38300bfdcd87a3056dc">
    [Paper]
  </a>
  <a >
    [RAGCap]
  </a>
  <a >
    [Dataset]
  </a>
</p>

---
## Abstract
Remote Sensing (RS) image captioning has traditionally relied on specialized models tailored to domain-specific tasks. The emergence of large vision-language models (VLMs) offers a promising alternative due to their versatility across tasks and domains. However, fine-tuning VLMs for specific applications introduces significant challenges, including computational overhead, overfitting risks, and reduced generalization capabilities. To address these limitations, we propose RAGCap a Retrieval-Augmented Generation framework that leverages pre-trained VLMs for RS captioning without the need for fine-tuning. Our approach employs a similarity-based retrieval model (SigLIP) to identify relevant image-caption pairs from the training set. These retrieved examples, along with the test image, are processed by a multi-image capable VLM (Qwen2VL) using a carefully designed prompt structure. This enables the model to generate captions that not only accurately describe the test image but also preserve the domain-specific style. Extensive evaluations on three RS benchmark datasets demonstrate that RAGCap achieves competitive performance compared to fine-tuned models while offering enhanced efficiency and generalization. Our framework provides a practical and scalable solution, maintaining the versatility of VLMs while effectively adapting to domain-specific requirements

## Architecture
<p align="center">
  <img width="600" src="https://github.com/BigData-KSU/RAGCap/blob/main/methodology_graph..png" alt="RAGCap Architectural Overview">
</p>

## Results
To evaluate RAGCap, we utilize three well-known benchmark RS datasets [xx]: Sydney, UCM, and NWPU Each image in these datasets is paired with five manually annotated captions. The Sydney dataset consists of 613 images, divided into 483 for training and 130 for testing. The UCM dataset includes 1,680 training images and 210 testing images. The NWPU dataset, the largest among them, contains 31,500 images, split into 25,200 for training and 6,300 for testing, with spatial resolutions ranging from 0.2 to 30 meters. 
We evaluate the method using standard captioning metrics, including BLEU (Bilingual Evaluation Understudy), ROUGE (Recall-Oriented Understudy for Gisting Evaluation), CIDEr (Consensus-based Image Description Evaluation), and SPICE (Semantic Propositional Image Captioning Evaluation). BLEU measures the precision of n-grams in the generated captions compared to the reference captions, focusing on word overlap. ROUGE emphasizes recall by evaluating phrase, n-gram, and sequence overlaps between generated and reference captions. CIDEr assesses the semantic relevance of captions using TF-IDF (Term Frequency-Inverse Document Frequency) weighted n-grams, rewarding captions that are both accurate and diverse. Finally, SPICE evaluates the semantic structure by comparing objects, attributes, and relationships in the captions, offering a deeper analysis of caption meaning beyond simple word matches. 


<p align="center">
  <img width="600" src="https://github.com/BigData-KSU/RAGCap/blob/main/Results_Table.png" alt="Results Table">
</p>

<p align="center">
  <img width="600" src="https://github.com/BigData-KSU/RAGCap/blob/main/Results_Graph.png" alt="Results Graph">
</p>

## Citation
Yakoub Bazi, Mohamad M. Al Rahhal, Mansour Zuair. RAGCap: Retrieval-Augmented Generation for Style-Aware Remote Sensing Image Captioning Without Fine-Tuning. Accepted for publication in IJRS (11-OCT-2025).   
 <p>
  <a Coming soon">
    DOI: 10.1080/01431161.2025.2575514 
  </a>
</p>
