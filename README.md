

# Comment Toxicity Detection using Deep Learning

## Table of Contents
### Overview
### Project Structure
### Installation
### Usage
### Model Architecture
### Data Preprocessing
### Evaluation
### References
### Sample Output

### Overview
This project aims to classify toxicity in comments using deep learning, specifically Natural Language Processing (NLP) and Long Short-Term Memory (LSTM) networks. The model uses a multi-label classification approach to detect multiple types of toxicity in online comments, inspired by the 2022 research of A. Garlapati, N. Malisetty, and G. Narayanan in the 8th ICACCS.

### Project Structure
Toxicity (1).ipynb - Main Jupyter notebook containing the data processing, model building, training, and evaluation steps.
data/ - Folder where the dataset (if available) should be stored.
models/ - Folder for saving model checkpoints or trained models.
utils.py - (Optional) Script with helper functions for data processing and model evaluation, if applicable.
### Installation
To set up this project, follow these steps:

### Clone this repository.
```python
git clone https://github.com/yourusername/toxicity-classification.git
cd toxicity-classification
```
Install dependencies:
```python
pip install -r requirements.txt
```
### Usage
1.Load the Dataset: Ensure the dataset is located in the data/ folder.


2.Run the Notebook: Open Toxicity (1).ipynb in Jupyter Notebook or Jupyter Lab and execute the cells in order.

### Model Architecture
The model architecture includes:
An Embedding Layer for word embeddings.
A Bidirectional LSTM Layer with 32 units to capture contextual information.
Dense Layers with 128, 256, and 128 units, respectively, for deep feature learning.
A final Dense Layer with 6 units and sigmoid activation for multi-label classification.

### Data Preprocessing
The preprocessing pipeline:
Tokenizes text data.
Pads sequences to a specified MAX_SEQUENCE_LENGTH.
Transforms text into vectorized input using a suitable vectorizer (e.g., TF-IDF).

### Evaluation
The model is compiled with:
Loss: Binary Crossentropy (for multi-label classification)
Optimizer: Adam
Use evaluation metrics such as accuracy, F1-score, and AUC-ROC to assess performance.

### References
Garlapati, A., Malisetty, N., & Narayanan, G. (2022). Classification of Toxicity in Comments Using NLP and LSTM. In 8th International Conference on Advanced Computing and Communication Systems (ICACCS).

### Sample Output
![image](https://github.com/user-attachments/assets/b83df21c-6007-4b84-afe0-fe5696e581bf)


