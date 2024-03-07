
<h2 align="center"> <a href="https://arxiv.org/abs/2402.13587">A Multimodal In-Context Tuning Approach for E-Commerce Product Description Generation</a></h2>

<p align="center"> 
  <a href="https://github.com/HITsz-TMG/Multimodal-In-Context-Tuning"> <img src="https://img.shields.io/badge/LingCloud-ModICT-brightgreen" height="18px" alt="ModICT">
  <a href="https://scholar.google.com/citations?user=U98QY0QAAAAJ&hl=en"><img src="https://img.shields.io/badge/scholar-4385FE.svg?&style=plastic&logo=google-scholar&logoColor=white" alt="Google Scholar" height="18px"> </a>
  <a href="https://twitter.com/LyxTg"> <img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" height="18px" alt="Yunxin Li">
</p> 

If you have any questions, please feel free to contact me by e-mail: liyunxin987@163.com, Twitter: [@LyxTg](https://twitter.com/LyxTg).

**The main contributions are:**

1) We present a product description generation paradigm that is based only on the image and several marketing keywords. For this new setting, we propose a straightforward and effective multimodal in-context tuning approach, named ModICT, integrating the power from the frozen language model and visual encoder.

2) Our work is the first one to investigate utilizing the in-context learning and text generation capabilities of various frozen language models for multimodal E-commerce product description generation. ModICT can be plugged into various types of language models and the training process is parameter-efficient.

3) We conduct extensive experiments on our newly built three-category product datasets. The experimental results indicate that the proposed method achieves state-of-the-art performance on a wide range of evaluation metrics. Using the proposed multimodal in-context tuning technical, small models also achieve competitive performance compared to LLMs.

## 🚀 Our Training Approach: ModICT

The overall workflow of ModICT. The left part depicts the process of in-context reference
construction. The right parts show the efficient multimodal in-context tuning ways for the sequence-to-
sequence language model (1) and autoregressive language model (2). Blocks with red lines are learnable.


![](https://github.com/HITsz-TMG/Multimodal-In-Context-Tuning/blob/main/product_model.png)




## 🤗 Our Proposed Dataset: MD2T
MD2T is a new setting for multimodal E-commerce Description generation based on structured keywords and images.

# MD2T Dataset Statistics

| MD2T      | Cases&Bags | Clothing | Home Appliances |
|-----------|------------|----------|-----------------|
| #Train    | 18,711     | 200,000  | 86,858          |
| #Dev      | 983        | 6,120    | 1,794           |
| #Test     | 1,000      | 8,700    | 2,200           |
| Avg_N #MP | 5.41       | 6.57     | 5.48            |
| Avg_L #MP | 13.50      | 20.34    | 18.30           |
| Avg_L #Desp | 80.05    | 79.03    | 80.13           |

**Table 1:** The detailed statistics of MD2T. Avg_N and Avg_L represent the average number and length respectively. MP and Desp indicate the marketing keywords and description.

Our preprocessed data (Text + Images) can be downloaded from https://huggingface.co/datasets/YunxinLi/MD2T.




## ✏️ Citation
If you find our paper and code useful in your research, please consider giving a star :star: and citation :pencil:.
```BibTeX
@article{li2024multimodal,
  title={A Multimodal In-Context Tuning Approach for E-Commerce Product Description Generation},
  author={Li, Yunxin and Hu, Baotian and Luo, Wenhan and Ma, Lin and Ding, Yuxin and Zhang, Min},
  journal={arXiv preprint arXiv:2402.13587},
  year={2024}
}
```
