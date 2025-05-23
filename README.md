# BiGTex
# Integrating Structural and Semantic Signals in Text-Attributed Graphs with BiGTex
The article can be viewed and downloaded from(https://arxiv.org/abs/2504.12474)

## Install requirements in  `requirements.txt`

## Download TAG datasets



| Dataset | Description |
| ----- |  ---- |
| ogbn-arxiv  | The [OGB](https://ogb.stanford.edu/docs/nodeprop/) provides the mapping from MAG paper IDs into the raw texts of titles and abstracts. <br/>Download the dataset [here](https://snap.stanford.edu/ogb/data/misc/ogbn_arxiv/titleabs.tsv.gz), move it to `datasets/arxiv`.|
| ogbn-products (subset) |  Download the dataset [here](https://drive.google.com/file/d/1F9D9NauJMlmwGcmLxhwbyAhfguWEZApA/view?usp=drive_link), unzip and move them to `datasets/products`.|
| arxiv_2023 |  Download the dataset [here](https://drive.google.com/file/d/1ekG96JHNPWqeQdb6D_GZoM28OGRLdcS_/view?usp=drive_link), unzip and move it to `datasets/arxiv_2023`.|
PubMed | Download the dataset [here](https://drive.google.com/file/d/1sYZX-jP6H8OkopVa9cp8-KXdEti5ki_W/view?usp=sharing), unzip and move it to `datasets/pubmed`.|

## Training and then save embeddings for BiGTex and ogbn-arxiv

```
python main.py 'arxiv' 'BiGTex'
```
you can run for other dataset: 'pubmed', 'products', 'arxiv_2023'
or other models: 'MLP', 'GCN', 'GAT', 'SAGE'

## BiGTex embeddings
You can download the generated embeddings by BiGTex [here ](https://drive.google.com/file/d/1RKJEHeN_lhO7drEd4KlofAqiTqmzSWEE/view?usp=drive_link).
unzip and move them to `embeddings`, so you can run more experiments like link prediction or clusstering using them.

##
## Citation
If you find our work useful, please consider citing our work:

```
@misc{beiranv2025integrating,
    title={Integrating Structural and Semantic Signals in Text-Attributed Graphs with BiGTex},
    author={Azadeh Beiranvand and Seyed Mehdi Vahidipour},
    year={2025},
    eprint={2504.12474},
    archivePrefix={arXiv},
    primaryClass={cs.CL}
}
``` 
