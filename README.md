# Transfer Learning with Pretrained CNNs

### How much do you actually need to retrain?

A machine learning tutorial exploring three transfer learning strategies applied to ResNet-18 on the Oxford 102 Flowers dataset.

\---

## Overview

Training a CNN from scratch requires massive data and compute. This tutorial demonstrates how **transfer learning** lets you achieve strong results with a small dataset by reusing features learned on ImageNet.

Three strategies are compared:

|Strategy|Layers Updated|Best For|
|-|-|-|
|A — Feature Extraction|Classifier head only|Small dataset, similar domain|
|B — Partial Fine-tuning|Last conv block + head|Medium dataset, moderate domain shift|
|C — Full Fine-tuning|All layers|Large dataset or big domain shift|

\---

## Quickstart

### 1\. Clone the repository

```bash
git clone https://github.com/gaurey/cnn-transfer-learning.git
cd cnn-transfer-learning
```

### 2\. Install dependencies



> \*\*GPU recommended\*\* — on CPU, each strategy takes \~30 min per 20 epochs.  
> On Google Colab (free GPU), each strategy takes \~2–3 min.  


### 3\. Run the notebook

```bash
jupyter notebook notebook/transfer\_learning\_tutorial.ipynb
```

The notebook will **automatically download** the Oxford 102 Flowers dataset (\~330 MB) on first run.

\---

## Requirements

* Python 3.8+
* PyTorch 2.0+
* torchvision 0.15+
* matplotlib 3.5+
* numpy 1.22+
* Pillow 9.0+
* tqdm 4.64+

\---

## Dataset

**Oxford 102 Flowers** (Nilsback \& Zisserman, 2008)  
102 flower categories, \~8,000 images total.  
Downloaded automatically via `torchvision.datasets.Flowers102`.  
Original dataset: https://www.robots.ox.ac.uk/\~vgg/data/flowers/102/

\---



## Accessibility

* All figures use the **Okabe-Ito colourblind-safe palette**
* Alt-text descriptions are included as comments in all figure-generating cells
* The PDF tutorial uses high-contrast colours and is structured for screen readers

\---

## Licence

This project is licensed under the **MIT Licence** — see [LICENSE](LICENSE) for details.  
You are free to use, modify, and distribute this code with attribution.



