# Welcome to the Vertex AI workshop

This codebase contains all you need to get started with the workshop. Please go to file **[start-version-vertex-ai-pipeline](https://github.com/devoteamgcloud/vtk-workshop-2023/blob/main/start-version-vertex-ai-pipeline.ipynb "start-version-vertex-ai-pipeline.ipynb")** and adapt it how you like. The goal is to create an endpoint that can be used by other people to get price estimates on houses based on the features of the house.


## TODO 1: make the model

In component "train_model" we lack the actual code to create and train an sklearn model. This model should take in all of the features and predict the value of the home. You are free to choose whichever sklearn model you like best but make sure it can handle the numeric and boolean features as well as the continuous output value.

**Note**: Vertex AI can also work with other AI-frameworks (PyTorch, Tensorflow ...) but these require small changes in other parts of the code hence the limitation of using an sklearn model in this exercise.

## TODO 2: use more features

Typically the more information available to the model, the better the predictions will be. In the table on BigQuery you can see that there is one column that is not used right now, called "furnishingstatus". This table is different from the rest and needs some preprocessing before it can be used in the training. Checkout the component process_source_data and try to change it so the model can also train on the furnishingstatus.

## Stuck?
We are happy to help you on your way so just give a shout :)
