# Machine Learning & Data Science
## What?
* The application of AI to provide systems with the ability to learn and improve from experience
* **Supervised Learning** - algorythm learns from *labeled* training data
    * learns what connects images of the same label
* **Unsupervised Learning** - algorythm learns from finding similar data points in data sets
    * unlabeled: explores data to try to find a hidden structure
* **Reinforcement Learning** - learn ideal behaviour within an environment
    * e.g. Try to get the highest score in a maze
## Machine vs Deep Learning
* Machine learning - A subset of artificial intelligence involved with the creation of algorithms which can modify itself without human intervention to produce desired output- by feeding itself through structured data.
* Deep learning - A subset of machine learning where algorithms are created and function similar to those in machine learning, but there are numerous layers of these algorithms- each providing a different interpretation to the data it feeds on. Such a network of algorithms are called artificial neural networks
* Example: picture of cats and dogs want to identify which is which
* Machine learning solution - label images (structured data) to define specific features of cats and dogs
      * System can use algorythm to analyse and learn these patterns ad can now classify other images
* Deep learning solution - The artificial neural networks using deep learning send the input (the data of images) through different layers of the network, with each network hierarchically defining specific features of images.
      * System able to classify both images based in identifiers (specific features)
**Reference for definitions and example: https://hackernoon.com/deep-learning-vs-machine-learning-a-simple-explanation-47405b3eef08**
## Applications
* Neural nets - for object recognition
* Deep speech - speech recognition
* Self drive cars
## Getting started
* Download anaconda 3 python distribution
* In anaconda prompt:
    * Navigate to directory with data (e.g. excel spreadsheet) and environment.yml (dependencies such as scikit-learn, matplotlib etc.)
    * **conda env create** - creates environmet from environment.yml
    * **conda activate <env-name>** - specified in yaml
    * **jupyter notebook** - launches environment in browser
## Modeling Data
1. Import relevant classes from keras
    * neural-network library runs on top of TensorFlow (numerical computation library)
    * **from keras.models import sequential**
2. Define the model
    * **model = Sequential()**
3. Add layer
    * **model.add(Dense(1, input_shape = (1, )))**
    * first number = n.o. output values
    * second number = n.o. features (find by X.shape -> return (XXXX, 1) therefore second number is 1
    * modal.Summary() to review
4. Compile model - keras constructs model using backend (e.g. tensorflow)
    * **model.compile(Adam(lr = 0.8), 'mean_squared_error')**
    * Adam = optimiser 
    * optimisers used to produce better and faster results by updating Weight and Bias values
    * https://towardsdatascience.com/types-of-optimization-algorithms-used-in-neural-networks-and-ways-to-optimize-gradient-95ae5d39529f
    * https://keras.io/optimizers/
    * 'mean_squared_error' = cost function
    * cost function calculate loss which represents difference between estimated and true values
5. Fit model - define n.o. epochs
    * epoch = entire processing by learning model of entire train set
    * **model.fit(X, y, epochs = 20)**
    * As fitting procedure runs loss decreases and accuracy increases
6. Use model
    * To plot contour (onto grid created using linespace)
    * To generate predictions (e.g. for X) and extract Weight and Bias
