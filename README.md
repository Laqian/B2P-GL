# B2P-GL
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

### Population Graph Constrcution Method

*Table 2: Performance comparison of phenotypic-brain feature similarity edge versus condition-based edge in graph construction.*

| Edge Construction Method              | Accuracy       | AUC           | Specificity   | Sensitivity   |
|----------------------------------------|----------------|---------------|---------------|---------------|
| Phenotypic-Brain Feature Similarity    | 81.95 ± 0.52   | 81.71 ± 0.51  | 85.29 ± 1.87  | 78.12 ± 1.85  |
| Condition-based                    | 83.40 ± 0.50   | 83.00 ± 0.30  | 88.90 ± 0.50  | 77.10 ± 0.10  |


*Table 3: Performance comparison of same-category versus different-category edge connections within conditions.*
| Edge Connection Type               | Accuracy   | AUC       | Sensitivity (Recall) | Specificity   |
|------------------------------------|------------|-----------|----------------------|---------------|
| Same-category edges               | 82.00 ± 0.54 | 81.67 ± 0.59 | 86.58 ± 0.73        | 76.77 ± 1.49  |
| Different-category edges          | 83.40 ± 0.50   | 83.00 ± 0.30  | 88.90 ± 0.50  | 77.10 ± 0.10  |


<br>
<br>

### Phenotypic Fusion Module

*Table 6: Performance comparison with and without phenotype feature fusion.*
| Feature Fusion    | Accuracy       | AUC           | Sensitivity   | Specificity   |
|------------------|----------------|---------------|---------------|---------------|
| No Fusion        | 77.06 ± 0.42   | 76.67 ± 0.36  | 82.08 ± 1.38  | 71.27 ± 1.05  |
| With Fusion      | 83.40 ± 0.50   | 83.00 ± 0.30  | 88.90 ± 0.50  | 77.10 ± 0.10  |

<br>
<br>



## Two-Stage Experiment

*Table Performance comparison with/without similarity loss in training stages.*

| Configuration          | Accuracy   | AUC       | Sensitivity | Specificity   |
|------------------------|------------|-----------|-------------|---------------|
| Stage 1 w/o similarity | 73.38 ± 0.92 | 72.77 ± 1.01 | 81.28 ± 1.59 | 64.26 ± 2.81  |
| Stage 1 w/ similarity  | 73.70 ± 0.60 | 73.20 ± 0.60 | 80.50 ± 1.80 | 65.90 ± 2.10  |
| Stage 2 w/o similarity | 81.95 ± 0.57 | 81.62 ± 0.60 | 86.60 ± 1.19 | 76.63 ± 1.46  |
| Stage 2 w/ similarity  | 83.40 ± 0.50 | 83.00 ± 0.30 | 88.90 ± 0.50 | 77.10 ± 0.10  |


