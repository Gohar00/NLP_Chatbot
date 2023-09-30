# Chatbot with NLP (Natural Language Processing)

__Overview__
This project is an implementation of a chatbot using Natural Language Processing (NLP) techniques. The chatbot is designed to answer questions posed by students. It utilizes a deep learning architecture with an encoder-decoder model, embedding layers, and LSTM (Long Short-Term Memory) cells. The chatbot has been trained on a dataset containing questions and answers, enabling it to provide responses to user queries.

__Prerequisites__
Before using the chatbot, ensure that you have the following prerequisites installed:

* Python 3.x
* TensorFlow 2.x
* Gensim (for Word2Vec)
* Pandas
* Numpy
* scikit-learn
* YAML
* Other necessary Python libraries

# Getting Started
__1. Clone the Repository:__

Clone this repository to your local machine.
* _git clone <repository_url>_ 
* _cd <repository_directory>_

**2. Install Dependencies:**

Install the required Python libraries by running the following command:
* _- pip install -r requirements.txt_
  
**3. Dataset Preparation:**
Place your dataset files in the archive directory.

**4. Data Preprocessing:**
Run the provided Jupyter Notebook or Python script to preprocess the data. This includes tokenization, padding, and one-hot encoding of the questions and answers.

**5. Model Training:**
Train the chatbot model by running the training script. You can adjust hyperparameters and training settings as needed.

**6. Inference:**
After training, you can use the chatbot to answer questions. The inference function allows you to interact with the chatbot and provide it with questions.

# Model Architecture
The chatbot model architecture consists of the following components:

* Encoder: Processes input questions and extracts meaningful representations using an LSTM layer.

* Decoder: Generates responses using another LSTM layer, taking the encoder's output as input.

* Embedding Layers: Used to convert words into numerical vectors.

* Dense Layer: The final layer that outputs the response in a one-hot encoded format.

# Usage
**1. Load the trained model by running:**
* _model = tf.keras.models.load_model('bot.h5')_
* _enc_model, dec_model = inference()_

**2.Use the preprocess_input function to convert user input into a format the model can understand.**

**3.Interact with the chatbot by providing input sentences using the enc_model and dec_model for encoding and decoding responses.**

**4.Sample interaction code is provided in the Jupyter Notebook or Python script to demonstrate how to use the chatbot.**
