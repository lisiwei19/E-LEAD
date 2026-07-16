# E-LEAD: Efficient LLM-Enhanced Node Anomaly Detection in Text-attributed Graphs

<img src="https://raw.githubusercontent.com/lisiwei19/E-LEAD/main/%E5%9B%BE%E7%89%872.png" width="100%">



## Datasets


The statistics of the datasets used in our experiments are shown below.

| Dataset | Nodes | Edges | Anomalies |
|:-------:|------:|------:|----------:|
| Cora | 2,708 | 10,984 | 108 |
| PubMed | 19,717 | 90,368 | 788 |
| History | 41,551 | 369,252 | 1,662 |
| Arxiv | 169,343 | 1,210,112 | 6,774 |


## Usage

### Train on Cora

``` bash
python run.py --dataset cora 
```

### Train on PubMed

``` bash
python run.py --dataset pubmed 
```

### Train on History

``` bash
python run.py  --dataset history 
```

### Train on Arxiv

``` bash
python run.py --dataset arxiv --ba_bf_backend sparse_lookup_batch 
```

### Test

``` bash
python run.py --mode test --dataset cora
```

## LLM Semantic Review

Set your API key:

``` bash
export API_KEY="your_api_key"
```

Enable LLM enhancement:

``` bash
python run.py --dataset cora --enable_llm_api
```

## Dependencies

-   Python 3.10
-   PyTorch 2.6.0
-   CUDA 12.6
-   PyTorch Geometric 2.7.0
-   DGL 1.1.3
-   Transformers 5.0.0
-   NumPy 2.2.6
-   SciPy 1.15.3
-  Pandas 2.3.3
-   Scikit-learn 1.7.2


## Citation

If you find this work useful, please cite:

``` bibtex
@article{elead2026,
  title={E-LEAD: Efficient LLM-Enhanced Node Anomaly Detection in Text-attributed Graphs},
  year={2026}
}
```
