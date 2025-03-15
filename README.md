# Topic modelling for Vietnamese product reviews
Result summary:
|   Feature representation          | BOW  | Tf-idf | Skip-gram | CBOW | PhoBERT |
|:-----------------------:|:----:|:----:|:----:|:----:|:----:|
| Best performing model  | CC-XGB | CC-XGB | CC-XGB | CC-XGB| BR-LR |
|       Hamming loss      |  0.049 | 0.05 | 0.071 | 0.066 | 0.022 |
|        Macro-F1        | 0.89 | 0.89 | 0.83 | 0.84 | 0.96 |
|          Micro-F1         | 0.92 | 0.92 |0.88 | 0.89 | 0.96 |
----------------------------------------------------------------
Demo Streamlit app: [HuggingFace Repo](https://huggingface.co/spaces/NTDuy/vietnamese-shopee-streamlit)
<br />
App screenshot:
![image](https://github.com/DDKson/THESIS_DSEB62-Product_review_analysis/assets/92723196/7e633598-68b7-46ed-a1ed-64943e6f6207)

