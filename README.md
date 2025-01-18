# Next Word Predictor

## Project Overview
The Next Word Predictor is a machine learning-based application that predicts the next word in a sequence of text. It uses an LSTM (Long Short-Term Memory) neural network trained on textual data from **"sherlock-holm.es_stories_plain-text_advs"**, enabling it to provide contextually relevant suggestions.

## Features
- Predicts the next word given a sequence of input text.
- Tokenization and preprocessing to prepare input text for prediction.
- Embedding and LSTM layers for effective learning of language patterns.

## Dataset
The dataset used is **"sherlock-holm.es_stories_plain-text_advs"**, a plain-text file containing stories of Sherlock Holmes. This dataset was tokenized and processed to create sequences for training the model.

## Technologies Used
- **Python**: Core programming language.
- **TensorFlow/Keras**: For building and training the LSTM model.
- **Flask**: For creating the API to host the model.
- **Numpy** and **Pandas**: For data manipulation and preprocessing.
- **Pickle**: To save and load the tokenizer.

## Installation and Setup
### Prerequisites
- Python 3.8 or higher
- Virtual environment setup (recommended)

### Steps
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd Next_Word_Predictor
   ```

2. Create and activate a virtual environment:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install required dependencies:
   ```bash
   pip install -r requirements.txt
   ```

4. Place the dataset file **"sherlock-holm.es_stories_plain-text_advs"** in the project directory.

5. Train the model (if needed):
   ```bash
   python train_model.py
   ```


## Model Details
The model is a sequential neural network with the following architecture:
- **Embedding Layer**: Converts words into dense vectors of fixed size.
- **LSTM Layer**: Captures long-term dependencies in the text.
- **Dense Layer with Softmax**: Outputs probabilities for the next word.

### Hyperparameters
- Vocabulary size: Based on the dataset tokenizer.
- Embedding dimensions: 100
- LSTM units: 200,150
- Max sequence length: 18

## Future Improvements
- Incorporate attention mechanisms to improve context understanding.
- Expand the dataset to include diverse textual sources.
- Deploy the application using cloud platforms like AWS or Render.
- Create a front-end interface for user-friendly interaction.

## Contributing
Contributions are welcome! Please fork the repository and submit a pull request.


