# Twitte-r-sentiment-prediction-using-Deep-Learning
Social media sentiment analysis 

Social media has been initially found to be a great platform of connecting people from all over the world and still remained in top position as a virtual medium among netzines however most of the media platforms (e.g. Twitter, Facebook, Instagram) over the years have been commercialized and democratized as well and that leads to an interesting research area where users opinions or participation can impact an organization’s or brand’s reputation in no time. Analyze unstructured users’ opinion or text in twitter platform and predict sentiments and discovering relations between part of text with sentiments using artificial intelligence algorithms known as deep learnings are the objectives of this paper. Successful AI model can work independently across different media platforms to predict users view or judgements, fake news, hate speech propagation etc.

Steps Performed - 
Data Preprocessing – Data is sourced from Kaggle twitter hosted sentiment analysis competition and following steps performed further. Google colab infrastructure and python language used for to develop the system.
1. Imported the required python libraries (e.g. numpy, pands, matplotlib, sklearn, keras (used for deep learning which works well and user friendly than another deep learning library tensor flow))
2. Imported dataset (twitter dataset) in google colab environment
3. Data exploration, handle missing data and data quality check (no missing data found and lowered all characters, and removed regular expressions)
4. Encoded independent categorical text data (words needed to embedded before LSTM can be applied hence twitter sentences converted to sequences using tokenizers function followed by padding operation to make fixed lengths (strings- tokens – integers - vectors)) – list of strings where each string is a single word and this process is called tokenization.
Building RNN – Recursive neural network training follows few more steps followed by prediction.
1. Applied LSTM and dense layer (SoftMax activation function is selected because this is multi classification problem, sigmoid works well with binary classification. Other two rectifier activation function and Hyperbolic tangent activation function works well with different problems)
2. Compiled the RNN model (categorical_crossentropy is selected because categorical prediction will be performed by model, binary_crossentropy is another choice for binary classification)
3. Convert dependent feature to indicator variables (get_dummies function used of panda library)
4. Distributed train and test data into 80/20 ration and trained the model with 20 epochs
Prediction and Evaluate Model – Trained model is used to test 20 percent of dataset kept aside earlier.
1. Tested records with the trained model and calculated accuracy.
2. Noted observations and hyper parameters.
Different hyperparameters have been attempted for recurrent neural networks and good enough parameters values kept in source code (placed as colab file in drive and link highlighted below).
