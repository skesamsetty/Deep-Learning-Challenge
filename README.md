# Alphabet Soup Charity - Funding predictor

## Background

Objective is to build a model for Alphabet Soup to predict whether applicants will be successful if funded by Alphabet Soup.

## Analysis

1. Initially the neural network was designed with following hyperparameters:

        Number of Hidden layers: 2 (excluding output layer)
        Layer 1:
            Units count (Nuerons): 80
            Activation functions : ReLU
            Input dimensions     : 43
        Layer 2:
            Units count (Nuerons): 30
            Activation functions : Tanh
        Output Layer:
            Units count : 1
            Activation  : Sigmoid
        Compile parameters: loss="binary_crossentropy", optimizer="adam"
        Epoch count: 50
        Model Score using test data: loss: 54.84% - accuracy: 73.46%

        Target variables: IS_SUCCESSFUL
        Features: APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT
        Other Variables: EIN, NAME

2. Optimization Attempt 1:
        
        Number of Hidden layers: 12 (excluding output layer)
        Layer 1:
            Units count (Nuerons): 80
            Activation functions : ReLU
            Input dimensions     : 43
        Layer 2:
            Units count (Nuerons): 30
            Activation functions : Tanh
        Layer 3 - 12:
            Units count (Nuerons): 30
            Activation functions : ReLU
        Output Layer:
            Units count : 1
            Activation  : Sigmoid
        Compile parameters: loss="binary_crossentropy", optimizer="adam"
        Epoch count: 50
        Model Score using test data: loss: 54.90% - accuracy: 73.67%

3. Optimization Attempt 2:
        
        Number of Hidden layers: 12 (excluding output layer)
        Layer 1:
            Units count (Nuerons): 80
            Activation functions : ReLU
            Input dimensions     : 43
        Layer 2:
            Units count (Nuerons): 30
            Activation functions : Tanh
        Layer 3 - 12:
            Units count (Nuerons): 30
            Activation functions : ReLU
        Output Layer:
            Units count : 1
            Activation  : Sigmoid
        Compile parameters: loss="binary_crossentropy", optimizer="adam"
        Epoch count: 50
        Model Score using test data: loss: 54.90% - accuracy: 73.67%