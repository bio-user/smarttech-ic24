# Enhancing Cellular Line Representation with Transformer-Based Text Embeddings for Precision Drug Repositioning

This repository contains the code and data used for the paper titled **"Enhancing Cellular Line Representation with Transformer-Based Text Embeddings for Precision Drug Repositioning"**. The project focuses on representing cellular lines using transformer-based models to aid in drug discovery and personalized medicine.

## Table of Contents
- [Introduction](#introduction)
- [Data](#data)
- [Methodology](#methodology)
- [Requirements](#requirements)
- [Usage](#usage)
- [Reproducibility](#reproducibility)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## Introduction
This project explores a novel approach to representing cellular lines using transformer-based embeddings. The embeddings are generated from PubMed abstracts related to various cellular lines, and clustering techniques are applied to identify biologically meaningful groupings that could enhance drug response prediction. The code provided here allows researchers to replicate the analysis and further develop the approach for similar applications.

## Data
The dataset used in this study consists of PubMed abstracts related to cellular lines, retrieved using a structured search query. The preprocessed dataset and the transformer-generated embeddings are available in the repository.

- **Corpus**: PubMed abstracts related to cellular lines.
- **Embeddings**: Sentence-level embeddings generated using the `SentenceTransformer('all-MiniLM-L6-v2')`.

## Methodology
1. **Data Collection**: Abstracts were retrieved from PubMed using structured queries focused on cellular lines. Synonym consolidation and text normalization were applied to standardize the data.
2. **Embedding Generation**: The abstracts were processed using the SentenceTransformer model to generate dense, contextual embeddings for each cellular line.
3. **Clustering**: Clustering algorithms (e.g., K-Means) were applied to group the embeddings based on semantic similarity.
4. **Evaluation**: Clustering quality was evaluated using the Topic Coherence metric, and t-SNE was used for visualization.

## Requirements
To replicate the results, you need the following packages:
- Python 3.8+
- `transformers` library
- `sentence-transformers`
- `scikit-learn`
- `matplotlib`
- `pandas`
- `numpy`

You can install all the required dependencies with:
```bash
pip install -r requirements.txt
```

## Usage
1. Clone the Repository

```bash
git clone https://github.com/bio-user/smarttech-ic24
```
2. Data Processing

Run the notebook from the notebooks/ folder
## Reproducibility

All the steps needed to reproduce the results in the paper are available in this repository. By following the instructions above, you can generate the same embeddings, apply the clustering methods, and visualize the results.

For detailed reproducibility, we recommend running the entire pipeline in sequence. The raw data and generated embeddings are also available for download within the repository to facilitate quick testing.

## Results

The results include:

* Embeddings: Dense, contextual representations of PubMed abstracts related to cellular lines.
* Clusters: 23 clusters representing biologically meaningful groupings of cellular lines.
* Visualization: t-SNE visualization of the clusters.

The final results and evaluation metrics can be found in the results/ folder.

## Contributing

Contributions are welcome! If you wish to contribute to this project, please fork the repository and submit a pull request. Make sure to adhere to the coding standards and document any changes.

## License

This project is licensed under the MIT License. See the LICENSE file for more details.