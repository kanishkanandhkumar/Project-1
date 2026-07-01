# Project-1
# Gene Prioritizer GNN

This repository contains the implementation of a Graph Neural Network (GNN) pipeline designed for oncogene prioritization. The model utilizes the human protein-protein interaction (PPI) network to identify genes critical to cancer pathogenesis.

## Technical Architecture
The model integrates structural topology with node classification to predict gene-disease associations.



## Performance Metrics
- **ROC-AUC:** 0.9347
- **Model Architecture:** Hybrid GCN/GAT
- **Interpretability:** GNNExplainer for feature importance mapping

## Implementation Details
The project utilizes PyTorch Geometric to perform message passing across the STRING interactome. Security constraints are handled via `weights_only=False` for graph data structures, ensuring robust serialization.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Contact
For inquiries regarding the research methodology or technical implementation, please contact the lead researcher.
