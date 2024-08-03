# HistoneWrapClassifier

This repository contains the documentation of our work in the course project of BITS 464 Machine Learning. The course introduced us to several fundamental concepts of Machine Learning such as regression, classification, neural networks, and SVMs. As part of our final project, we created this repository.

## Project Overview

The goal of this project is to classify whether histones wrap around DNA sequences or not using deep learning techniques. Histones are proteins that help in the organization and packaging of DNA into structural units called nucleosomes. Understanding histone-DNA interactions is crucial for insights into gene regulation and epigenetics. Inspired by the paper ["DNA Sequence Classification by Convolutional Neural Network" by Nguyen et al.](https://www.scirp.org/journal/paperinformation?paperid=65923), we carried out our research and implemented various models to achieve this classification.

## Steps Followed for Implementation

Due to the computational resources available, we selected the H3K4me1 dataset out of the 12 mentioned in the paper. A broad overview of our approach is below:

- Performed exploratory analysis to understand the dataset and removed any noise present.
- Implemented 3-mer representation and one-hot encoding embedding method for each sequence.
- Replicated the model architecture from the paper and selected the best hyperparameters.
- The dataset used and the code for base model implementation can be found in this repository.

## Further Changes Made

To develop a novel approach, we brainstormed and divided the project into three segments:
- Sequence Representation
- Sequence Embedding
- Model Architecture

We started experimenting with each segment. All the successful experiments have been documented, including:

1. Hyperparameter Tuning
2. Utilization of 4-mer representation
3. Utilization of Word2Vec embedding
4. Utilization of Hybrid models

Code used for every model has been attached in the repository.

## Repository Structure

- `HK4me1.txt`: Contains the raw dataset used.
- `dataset.txt`: Is the cleaned dataset after preprocessing.
- `OnehotEncoding_CNN.ipynb`: Jupyter notebook for base model implementation.
- `OnehotEncoding_CNN_hyperparam_optim.ipynb`: Jupyter notebook for hyperparameter tuning of base model cnn.
- `onehot_cnn+bilstm.ipynb`: Jupyter notebook for hybrid model.
- `word2vec_cnn+bilstm.ipynb`: Jupyter notebook for Word2Vec embedding and hybrid model implementation.
- `4mer_Word2Vec_CNN+LSTM.ipynb`: Jupyter notebook for 4mer representation and hybrid model.
- `README.md`: Project overview and instructions.
- `ML Project Report (1).pdf` : Project report.
- `ML Project Presentation.pdf`: Presentation.

## Installation

1. Clone the repository:
    ```bash
    git clone https://github.com/bug-slayer07/Histone_Wrap.git
    cd Histone_Wrap
    ```

2. Install the required libraries:
    ```bash
    pip install -r requirements.txt
    ```

## Running the Project

1. Ensure the dataset is in the `data/` directory.
2. Open and run the Jupyter notebooks in the repository to replicate our experiments and models.

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or new features.

## License

This project is licensed under the MIT License. See the `LICENSE` file for details.

## References

- [DNA Sequence Classification by Convolutional Neural Network](https://www.scirp.org/journal/paperinformation?paperid=65923)

## Contributors

- [Mridul Mishra](https://github.com/bug-slayer07)
- [Shireen Shaikh](https://github.com/toasted-breads-2)
