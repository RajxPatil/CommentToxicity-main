# Comment Toxicity Detection

This project implements a machine-learning model for detecting toxicity in comments. The model can identify toxic language across various categories, such as hate speech, insults, threats, and more. Built using natural language processing (NLP) techniques, this model aims to create safer and more inclusive online communities.

## Features

- **Pre-trained NLP model:** Uses transfer learning to process and classify text comments efficiently.
- **Multi-label classification:** Detects various forms of toxicity, including threats, insults, obscenities, and hate speech.
- **Interactive UI:** Provides a web-based interface to allow users to test the model's performance.
- **Scalable architecture:** Can be deployed in real-time applications for comment moderation or analysis.

## Getting Started

### Prerequisites

- Python 3.7+
- Install the following Python libraries:
  ```bash
  pip install tensorflow pandas numpy sklearn
  ```

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/nicknochnack/CommentToxicity.git
   cd CommentToxicity
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. (Optional) If you'd like to work with Jupyter notebooks, you can install Jupyter:
   ```bash
   pip install notebook
   ```

### Running the Project

#### Training the Model

1. Open the `toxicity_model_training.ipynb` notebook to train the model using the dataset.
2. Use the [Jigsaw Toxic Comment Classification Dataset](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/data).
3. Train the model and save it for future use.

#### Running the Web Application

1. After training the model, you can run the web application to detect comment toxicity:
   ```bash
   python app.py
   ```
   
## Usage

- Enter a comment in the web app, and the model will predict whether the comment contains toxic elements such as threats, obscenities, insults, or hate speech.
- The application outputs the probabilities for each toxicity label, allowing you to see the intensity of toxicity in the comment.

## Model Architecture

- **Embedding Layer:** Text input is converted to a dense vector representation.
- **LSTM Layer:** Processes the sequential nature of text and captures context for better understanding.
- **Fully Connected Layers:** Outputs probabilities for each toxicity label.

## Dataset

The model is trained on the [Jigsaw Toxic Comment Classification Dataset](https://www.kaggle.com/c/jigsaw-toxic-comment-classification-challenge/data), which contains thousands of labeled comments.

## Contributing

If you would like to contribute to this project, open a pull request or raise issues for bugs or improvements. Contributions are welcome!

---

Let me know if you'd like any further customization!
