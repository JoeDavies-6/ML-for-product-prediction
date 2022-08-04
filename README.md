# ML-for-product-prediction
The code within this project is found within a collection of IPython Notebooks.
The files are split into the following sections:
  - Data
  - Non-neural network methods
  - Neural network methods

Both the non-neural network and neural network methods include code to perform a cross-validation

The neural network methods also includes three use cases aimed at realistic scenarios:
  - Use case one: Takes the last chronological run (Crocus-025) as a test run and all earlier data as training data.
  - Use case two: Assess the potential to identify failed reaction runs (Crocus-017). A challenge for this use case is scenarios such as failure are important to identify, but make up a much smaller proportion of the training data. To address this, the smogn algorithm is employed to identify which datapoints are underrepresented in the training data. (https://github.com/nickkunz/smogn)
  - Use case three: This builds on use case one, but applies the logic to all runs after the first two. This uses each run as a test run but only using chronoloigcally earlier runs as training data. This allows for exploration of the relationship between prediciton accuracy and volume of training data, the distribtuion of the data space, and the model's ability to generalise.
