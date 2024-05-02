# CodeBERT

## Model Arch

![MERT-7](https://github.com/xinyueli2896/CodeBERT/assets/144223393/33859b7e-dd24-4a3b-bbee-cbaea04570d2)

Before you run,
1. install the packages with requirement.txt
2. you can either follow the instruction below to run a series of .py files or go with a single notebook 
3. the intermediate files you will be needing have already been created for you at foler [operational](https://github.com/xinyueli2896/CodeBERT/main/operational/) and [relational](https://github.com/xinyueli2896/CodeBERT/main/relational/), if you don't want to go through with it, skip to step 3 to train probe step directly

## [1.get_tokenized_dataset](https://github.com/xinyueli2896/CodeBERT/main/get_tokenized_dataset.py)

```
python get_tokenized_dataset.py --task YOUR_TASK
```

run this with setting the YOUR_TASK as 'operaitonal' or 'relational'

## [2.get_activations](https://github.com/xinyueli2896/CodeBERT/main/get_activations.py)
```
python get_activations.py --task YOUR_TASK
```

run this with setting the YOUR_TASK as 'operaitonal' or 'relational'

## [3.train_probes](https://github.com/xinyueli2896/CodeBERT/main/train_probes.py)
```
python train_probes.py --task YOUR_TASK --probe_type PROBE_TYPE
```

run this with setting the YOUR_TASK as 'operaitonal' or 'relational' and PROBE_TYPE as Linear or NonLinear

## visualize your results 
visual your results in https://github.com/xinyueli2896/CodeBERT/main/bert_code_probing.ipynb
