# Topic classification of vietnamese product reviews in e-commerce using PhoBERT
This repository provides source code for our [paper](https://link.springer.com/article/10.1057/s41270-025-00402-w):

    @article{nguyen2025topic,
    title={Topic classification of vietnamese product reviews in e-commerce using PhoBERT},
    author={Nguyen, Tuan Duy and Nguyen, Duc Minh and Nguyen, Huu Manh and Nguyen, Thi Quynh Giang},
    journal={Journal of Marketing Analytics},
    pages={1--15},
    year={2025},
    publisher={Springer}
    }
If you find this repository useful in your research, please consider citing our paper.

## 🧩 Methodology Summary
1. **Topic Modelling**  
   - Extract general topics and their related keywords from dataset of customer review.  
   - Experimented with topic modelling models: LDA ([Blei et al, 2003](https://www.jmlr.org/papers/volume3/blei03a/blei03a.pdf)), (BERTopic [Grootendorst, 2022](https://arxiv.org/abs/2203.05794))
2. **Topic Classification**
   - Classify reviews based on identified topics.
   - Experimented models: Bag-of-words, Tf-idf, Word2Vec ([Mikolov et al., 2013](https://arxiv.org/abs/1301.3781)), PhoBERT ([Nguyen et al., 2020](https://arxiv.org/abs/2003.00744))


## 📊 Results Summary
* CC-XGB: Classifier Chain + XGBoost model
* BR-LR: Binary Relevance + Logistic Regression
* Evaluation metric: Hamming Loss

|   Feature representation          | BOW  | Tf-idf | Skip-gram | CBOW | PhoBERT |
|:-----------------------:|:----:|:----:|:----:|:----:|:----:|
| Best performing model  | CC-XGB | CC-XGB | CC-XGB | CC-XGB| BR-LR |
|       Hamming loss      |  0.049 | 0.05 | 0.071 | 0.066 | 0.022 |
|        Macro-F1        | 0.89 | 0.89 | 0.83 | 0.84 | 0.96 |
|          Micro-F1         | 0.92 | 0.92 |0.88 | 0.89 | 0.96 |
----------------------------------------------------------------
Downloadable classification model: [HuggingFace Model](https://huggingface.co/NTDuy/Phobert-base-v2-shopee)
<br />
Demo Streamlit app: [HuggingFace Repo](https://huggingface.co/spaces/NTDuy/Vietnamese-review-classification)
<br />
App screenshot:
![image](https://github.com/DDKson/THESIS_DSEB62-Product_review_analysis/assets/92723196/7e633598-68b7-46ed-a1ed-64943e6f6207)


