### What is Neural Network?
* A neural network is a type of **Machine Learning** process, called deep learning, that uses **interconnected** nodes or neurons in a layered structure that resembles the human brain. It creates an adaptive system that computers use to learn from their mistakes and improve continuously.  
* This project applies three types of Neural Network (**RNN, CNN, MLP**) for Text Classification and compares their performance, such as accuracy on test data.  
* The dataset has already been labeled as "positive" or "negative".

---
  
<dl>
  <b>Data Preprocessing</b>
  <dd>Remove Punctuation, Count Unique Words, Average Review Length, Tokenization, Truncate and Zero-pad Review</dd>
  
  <b>Word Embedding</b>
  <dd>Embedding Layer with Top 5000 words, Flatten the Matrix to Vector</dd>
</dl>



---

### Models  
<dl>
  <dt><b>Multi-Layer Perceptron (MLP)</b></dt>
  <dd>Data is fed to the input layers and there may be one or more hidden layers, in which use nonlinear activation functions, allowing the network to learn data patterns and making predictions on the output layer.</dd>
  <dd>MLP is a <b>feed-forward</b> Neural Network.</dd>
  </dl>

<img width="604" alt="Screen Shot 2024-04-14 at 6 55 16 AM" src="https://github.com/Cxy990605/Neural-Network-for-Sentiment-Analysis/assets/99168940/f8f389c2-1782-4bbd-9f36-5799833c8712">


<dl>
  <dt><b>Convolutional Neural Networks (CNN)</b></dt>
  <dd>CNN can capture the spatial dependencies of an <b>image</b> thtough a seris of filters (kernels). It can determine elements by looking at various neignborhoods of the pixel in the image. </dd>  
  <dd>Convolution layers extract features such as edges and clors  and pooling layers apply dimensionality reduction for the most prominent features. Lastly, the results are mapped into the final output by fully connected layer.</dd>
  <dd>CNN is a <b>feed-forward</b> Neural Network.</dd>
  </dl>
  
<img width="700" alt="Screen Shot 2024-04-14 at 6 53 38 AM" src="https://github.com/Cxy990605/Neural-Network-for-Sentiment-Analysis/assets/99168940/31c5d4c7-1b1d-4710-bcdd-3fc6c29e5017">


<dl>
  <dt><b>Recurrent Neural Network (RNN)</b></dt>
  <dd>RNN works with <b>sequence</b> prediction problems, in which what will happen in the next stage is related to the current stage, but not as related to the first stage.</dd>
  <dd>RNN can handle arbitrarily input and output lenghts and use the internal memory to process arbitrary sequences of data.</dd>
  </dl>

<img width="519" alt="Screen Shot 2024-04-14 at 5 58 30 AM" src="https://github.com/Cxy990605/Neural-Network-for-Sentiment-Analysis/assets/99168940/2959f0a4-baa6-44e4-9e70-18d1f5f3ccd1">

---  
### Result

Models | Training Accuracy | Test Accuracy
--- | --- | ---
`MLP` | 0.9314 | 0.6467
`CNN` | 0.838 | 0.592
`RNN` | **0.997** | **0.732**

---



