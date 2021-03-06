Classifying Radio Signals from Space is divided into following tasks:

The data set is available in images, the actual radio signal (time series data) is transformed to 2D spectrogram images & the data set is downloaded from the seti.org site. 
There are four classes of signals in the dataset:
  1. Squiggle
  2. Narrowband
  3. Narrowband DRD
  4. Noise

Task 1:
  Importing essential modules and helper functions from NumPy, Matplotlib, and Keras.
Task 2: Load and Preprocess SETI Data
  Displaying 2D spectrograms using Matplotlib.
  Reshapeing the input data with NumPy.
Task 3: Creating Training and Validation Data Generators
  Generating batches of tensor image data with real-time data augmentation.
  Specifying paths to training and validation image directories and generating batches of augmented data.
Task 4: Creating a Convolutional Neural Network (CNN) Model
  Designing a convolutional neural network with 2 convolution layers and 1 fully connected layers to predict four signal types.
  Using Adam as the optimizer, categorical crossentropy as the loss function, and accuracy as the evaluation metric.
Task 5: Learning Rate Scheduling and Compile the Model
  When training a model, it is often recommended to lower the learning rate as the training progresses.
  Applying an exponential decay function to the provided initial learning rate.
Task 6: Train the Model
  Training the CNN by invoking the model.fit() method.
  Using ModelCheckpoint() to save the weights associated with the higher validation accuracy after every epoch
  Displaying live training loss and accuracy plots in Jupyter Notebook using livelossplot.
Task 7: Evaluate the Model
  Evaluating the CNN by invoking the model.fit() method.
  Obtaining the classification report to note the precision and recall of your classifier.
