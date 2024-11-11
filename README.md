<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Next-Word Text Predictor using LSTM - README</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 20px;
            color: #333;
        }
        h1, h2, h3 {
            color: #2c3e50;
        }
        ul {
            padding-left: 20px;
        }
        .container {
            max-width: 800px;
            margin: auto;
        }
    </style>
</head>
<body>
    <div class="container">
        <h1>Next-Word Text Predictor using LSTM</h1>
        <p>This project is a next-word text prediction model developed using Long Short-Term Memory (LSTM) neural networks. The model has been trained on custom textual data extracted from a research paper, and it is designed to predict the next word in a sequence, achieving an accuracy of 96.33%.</p>

<h2>Table of Contents</h2>
        <ul>
            <li><a href="#project-overview">Project Overview</a></li>
            <li><a href="#project-workflow">Project Workflow</a>
                <ul>
                    <li><a href="#data-gathering">Data Gathering</a></li>
                    <li><a href="#data-preprocessing">Data Preprocessing</a></li>
                    <li><a href="#model-building">Model Building</a></li>
                    <li><a href="#model-training">Model Training</a></li>
                    <li><a href="#model-evaluation">Model Evaluation</a></li>
                </ul>
            </li>
            <li><a href="#usage">Usage</a></li>
            <li><a href="#results">Results</a></li>
            <li><a href="#conclusion">Conclusion</a></li>
        </ul>

<h2 id="project-overview">Project Overview</h2>
        <p>The goal of this project is to predict the next word in a sequence of text using an LSTM neural network. This model has applications in predictive typing and other language modeling tasks.</p>
        <h2 id="project-workflow">Project Workflow</h2>
        <h3 id="data-gathering">1. Data Gathering</h3>
        <p>The data for this project was collected from a research paper. Relevant text was extracted to build a dataset that would provide coherent sentence structures for effective next-word prediction.</p>
        <h3 id="data-preprocessing">2. Data Preprocessing</h3>
        <p>In this step, the text data was structured to prepare it for model training:</p>
        <ul>
            <li><strong>Tokenization</strong>: The extracted text was tokenized using Keras' Tokenizer, transforming words into integer sequences.</li>
            <li><strong>Sequence Conversion</strong>: The text sequences were converted to numerical sequences.</li>
            <li><strong>Padding</strong>: Sequences were padded to match the length of the longest sentence in the dataset, ensuring uniform input shape for the model.</li>
            <li><strong>Feature and Label Extraction</strong>: The input (<code>X</code>) and output (<code>Y</code>) pairs were derived from the sequences to prepare the data for supervised learning.</li>
        </ul>
        <h3 id="model-building">3. Model Building</h3>
        <p>The model was built using an LSTM layer with 150 nodes, followed by a Dense layer with a softmax activation function. This configuration is well-suited for sequence prediction tasks and leverages LSTM's capabilities to capture temporal dependencies in text data.</p>
        <h3 id="model-training">4. Model Training</h3>
        <p>The model was compiled using the Adam optimizer for efficient training. Training was conducted over 100 epochs with the padded text sequences, achieving a high accuracy of 96.33%.</p>
        <h3 id="model-evaluation">5. Model Evaluation</h3>
        <p>After training, the model's performance was evaluated based on its accuracy and ability to predict the next word in a given sequence.</p>
        <h2 id="usage">Usage</h2>
        <p>To use the model, input a sequence of text, and the model will output the most probable next word based on the training data.</p>
        <h2 id="results">Results</h2>
        <p>The LSTM model achieved a prediction accuracy of 96.33%, demonstrating strong performance in next-word prediction for the dataset.</p>
        <h2 id="conclusion">Conclusion</h2>
        <p>This project showcases the effectiveness of LSTM networks in text prediction tasks. With further training on diverse datasets, this model can be adapted for various NLP applications, including predictive text keyboards and conversational agents.</p>
    </div>
</body>
</html>
