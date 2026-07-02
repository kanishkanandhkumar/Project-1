# Graph-OncoPriority

Graph-OncoPriority is a computational framework leveraging Graph Neural Networks (GNNs) to identify potential oncogenes by analyzing the structural topology of the human protein-protein interaction (PPI) network. By modeling gene-disease associations as a node classification problem, this project captures functional dependencies often overlooked by traditional statistical methods.



## Research Objective
The goal is to accurately prioritize candidate oncogenes within large-scale protein interactomes. This framework provides a scalable approach to biomarker discovery and therapeutic target identification.

## Methodology
The model utilizes a hybrid architecture of Graph Convolutional Networks (GCNs) and Graph Attention Networks (GATs) to perform message passing across the STRING protein interactome.

1. **Data Preprocessing:** Integration of high-confidence interaction networks and gene feature extraction.
2. **Model Architecture:** Implementation of multi-layer GNNs designed to aggregate neighborhood structural features.
3. **Interpretability:** Integration of GNNExplainer to decompose model predictions and map critical interactions to canonical signaling pathways.

## Key Performance Metrics
* **ROC-AUC:** 0.9347
* **Framework:** PyTorch Geometric
* **Explainability:** Node-level subgraph feature importance mapping

## Repository Structure
```text
├── data/               # Raw PPI datasets and preprocessed graph snapshots
├── results/            # Performance metrics, model weights, and visualizations
├── src/                # Core implementation (training, evaluation, explainability)
├── docs/               # Technical documentation and research notes
├── LICENSE             # MIT License
└── README.md           # Project documentation


Setup & Installation
Bash
# Clone the repository
git clone [https://github.com/kanishkanandhkumar/Project-1.git](https://github.com/kanishkanandhkumar/Project-1.git)

# Install dependencies
pip install torch torch_geometric pandas scikit-learn

License
This project is licensed under the MIT License - see the LICENSE file for details.

Citation
If you utilize this framework for your research, please cite the repository accordingly.
