# Supplementary Experiments
<br>

## Stage 1 Experiment

### Node Reassignment Module
*Table 1: Ablation study of node reassignment module in ANR-GAT. Top: complete removal. Middle: replacement with WGAT layer. Bottom: our full proposed model.*

| Model Variant                     | Accuracy       | AUC           | Specificity   | Sensitivity   |
|-----------------------------------|----------------|---------------|---------------|---------------|
| ANR-GAT (w/o node reassignment)   | 70.56 ± 0.54   | 70.43 ± 0.44  | 72.18 ± 4.02  | 68.68 ± 3.86  |
| ANR-GAT (WGAT → node reassignment) | 72.07 ± 0.12   | 71.20 ± 0.08  | 83.97 ± 2.21  | 58.43 ± 2.30  |
| ANR-GAT                       | 73.70 ± 0.60   | 73.20 ± 0.60  | 80.50 ± 1.80  | 65.90 ± 2.10  |

<br>
<br>

## Stage 2 Experiment

### Population Graph Construction Method

*Table 2: Performance comparison of phenotypic-brain feature similarity edge versus condition-based edge in graph construction.*

| Edge Construction Method              | Accuracy       | AUC           | Specificity   | Sensitivity   |
|----------------------------------------|----------------|---------------|---------------|---------------|
| Phenotypic-Brain Feature Similarity    | 81.95 ± 0.52   | 81.71 ± 0.51  | 85.29 ± 1.87  | 78.12 ± 1.85  |
| Condition-based                    | 83.40 ± 0.50   | 83.00 ± 0.30  | 88.90 ± 0.50  | 77.10 ± 0.10  |


<br>
<br>

*Table 3: Performance comparison of same-category versus different-category edge connections within conditions.*
| Edge Connection Type               | Accuracy   | AUC       | Sensitivity (Recall) | Specificity   |
|------------------------------------|------------|-----------|----------------------|---------------|
| Same-category edges               | 82.00 ± 0.54 | 81.67 ± 0.59 | 86.58 ± 0.73        | 76.77 ± 1.49  |
| Different-category edges          | 83.40 ± 0.50   | 83.00 ± 0.30  | 88.90 ± 0.50  | 77.10 ± 0.10  |


<br>
<br>


*Table 4: Performance metrics across different top-k values for ABIDE I dataset.*

| Top-k | Accuracy       | AUC           | Specificity   | Sensitivity   |
|-------|----------------|---------------|---------------|---------------|
| 1     | 82.59 ± 0.72   | 82.33 ± 0.81  | 86.03 ± 1.66  | 78.62 ± 2.74  |
| 2     | 82.45 ± 0.31   | 82.10 ± 0.36  | 87.08 ± 1.20  | 77.12 ± 1.71  |
| 3     | 82.52 ± 0.30   | 82.22 ± 0.38  | 86.44 ± 1.62  | 78.01 ± 2.09  |
| 4     | 82.64 ± 0.52   | 82.33 ± 0.52  | 86.93 ± 1.37  | 77.72 ± 1.50  |
| 5     | 83.41 ± 0.35   | 83.01 ± 0.33  | 88.88 ± 0.54  | 77.13 ± 0.11  |
| 6     | 82.64 ± 0.44   | 82.28 ± 0.37  | 87.44 ± 1.62  | 77.13 ± 1.13  |
| 7     | 82.59 ± 0.37   | 82.35 ± 0.38  | 85.53 ± 1.08  | 79.16 ± 1.25  |

*Table 4: Performance metrics across different top-k values for ADHD-200 dataset.*

| Top-k | Accuracy       | AUC           | Sensitivity   | Specificity   |
|-------|----------------|---------------|---------------|---------------|
| 1     | 77.02 ± 0.26   | 77.14 ± 0.25  | 80.27 ± 1.17  | 74.01 ± 1.22  |
| 2     | 77.61 ± 0.67   | 77.67 ± 0.67  | 79.33 ± 1.23  | 76.01 ± 0.96  |
| 3     | 78.74 ± 0.82   | 78.74 ± 0.84  | 78.67 ± 2.07  | 78.81 ± 1.53  |
| 4     | 78.95 ± 0.57   | 78.93 ± 0.63  | 78.44 ± 2.44  | 79.43 ± 1.54  |
| 5     | 78.53 ± 0.63   | 78.50 ± 0.57  | 77.82 ± 1.81  | 79.18 ± 2.48  |
| 6     | 78.76 ± 0.51   | 78.77 ± 0.50  | 78.89 ± 1.95  | 78.65 ± 2.00  |
| 7     | 78.08 ± 0.61   | 78.16 ± 0.67  | 80.36 ± 2.85  | 75.96 ± 2.12  |


### Phenotypic Fusion Module

*Table 6: Performance comparison with and without phenotype feature fusion.*
| Feature Fusion    | Accuracy       | AUC           | Sensitivity   | Specificity   |
|------------------|----------------|---------------|---------------|---------------|
| No Fusion        | 77.06 ± 0.42   | 76.67 ± 0.36  | 82.08 ± 1.38  | 71.27 ± 1.05  |
| With Fusion      | 83.40 ± 0.50   | 83.00 ± 0.30  | 88.90 ± 0.50  | 77.10 ± 0.10  |

<br>
<br>


### Population Graph Neural Network

*Table x: Performance comparison between GCN and HGCN architectures on condition-based graphs.*

| Model | Accuracy       | AUC           | Specificity   | Sensitivity   |
|-------|----------------|---------------|---------------|---------------|
| GCN   | 79.32 ± 0.48   | 78.90 ± 0.45  | 82.15 ± 1.20  | 75.80 ± 1.10  |
| HGCN  | 83.40 ± 0.50   | 83.00 ± 0.30  | 88.90 ± 0.50  | 77.10 ± 0.10  |


## Two-Stage Experiment

*Table x Performance comparison with/without similarity loss in training stages.*

| Configuration          | Accuracy   | AUC       | Sensitivity | Specificity   |
|------------------------|------------|-----------|-------------|---------------|
| Stage 1 w/o similarity | 73.38 ± 0.92 | 72.77 ± 1.01 | 81.28 ± 1.59 | 64.26 ± 2.81  |
| Stage 1 w/ similarity  | 73.70 ± 0.60 | 73.20 ± 0.60 | 80.50 ± 1.80 | 65.90 ± 2.10  |
| Stage 2 w/o similarity | 81.95 ± 0.57 | 81.62 ± 0.60 | 86.60 ± 1.19 | 76.63 ± 1.46  |
| Stage 2 w/ similarity  | 83.40 ± 0.50 | 83.00 ± 0.30 | 88.90 ± 0.50 | 77.10 ± 0.10  |


