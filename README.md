# Topic modelling for Vietnamese product reviews
This repository provides source code for our [paper](https://link.springer.com/article/10.1057/s41270-025-00402-w):

    @article{nguyen2025topic,
    title={Topic classification of vietnamese product reviews in e-commerce using PhoBERT},
    author={Nguyen, Tuan Duy and Nguyen, Duc Minh and Nguyen, Huu Manh and Nguyen, Thi Quynh Giang},
    journal={Journal of Marketing Analytics},
    pages={1--15},
    year={2025},
    publisher={Springer}
  }

Result summary:
* CC-XGB: Classifier Chain + XGBoost model
* BR-LR: Binary Relevance + Logistic Regression

|   Feature representation          | BOW  | Tf-idf | Skip-gram | CBOW | PhoBERT |
|:-----------------------:|:----:|:----:|:----:|:----:|:----:|
| Best performing model  | CC-XGB | CC-XGB | CC-XGB | CC-XGB| BR-LR |
|       Hamming loss      |  0.049 | 0.05 | 0.071 | 0.066 | 0.022 |
|        Macro-F1        | 0.89 | 0.89 | 0.83 | 0.84 | 0.96 |
|          Micro-F1         | 0.92 | 0.92 |0.88 | 0.89 | 0.96 |
----------------------------------------------------------------
Demo Streamlit app: [HuggingFace Repo](https://huggingface.co/spaces/NTDuy/Vietnamese-review-classification)
<br />
App screenshot:
![image](https://github.com/DDKson/THESIS_DSEB62-Product_review_analysis/assets/92723196/7e633598-68b7-46ed-a1ed-64943e6f6207)

