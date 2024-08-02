# I - PyTorch Fundamentals Practice

Welcome to the PyTorch Fundamentals practice notebook! This notebook is designed to help you strengthen your understanding of the basic concepts of PyTorch, a powerful open-source machine learning library for Python.

## Requirements

Before starting the exercises, ensure you are comfortable with the following:

- **Basic Python programming**: Familiarity with Python syntax and data structures.
- **Basic understanding of Tensors**: A fundamental concept in PyTorch.
- **Familiarity with NumPy**: Although not mandatory, knowing NumPy can be helpful since PyTorch is similar to NumPy in many ways.
- **Basic concepts of machine learning**: Not required but beneficial for understanding PyTorch concepts more easily.

## Instructions

1. **Read Each Exercise**: Each exercise consists of a question and a corresponding code cell for your answer.
2. **Write Your Solution**: Implement your solution in the provided code cell.
3. **Run Evaluation Code**: After writing your solution, run the evaluation code to check your answer. The evaluation code cell is provided after each exercise.
4. **Do Not Modify Evaluation Code**: Avoid modifying the evaluation code as it may lead to incorrect results.

# II - Exercise: Implementing a Simple Linear Regression Model with PyTorch

## Introduction

In this exercise, we will implement a simple linear regression model using PyTorch, a popular open-source machine learning library. Linear regression is a fundamental algorithm in machine learning used to predict a target variable by fitting the best linear relationship between the dependent and independent variables.

## Requirements

To complete this exercise, you need to:

1. **Import the Necessary Libraries**: Ensure you have the required PyTorch libraries imported.
2. **Prepare the Data**: Create tensors for our input data (`x`) and output data (`y`). For simplicity, we will use a linear relationship \( y = 2x + 1 \).
3. **Initialize the Parameters**: Initialize our weight (`w`) and bias (`b`) using `torch.nn.Parameter`. `torch.nn.Parameter` is a type of Tensor that is automatically added to the list of its module’s parameters.
4. **Define the Model**: Implement a simple linear model: \( y = wx + b \).
5. **Define the Loss Function**: Use Mean Squared Error (MSE) as our loss function.
6. **Train the Model**: Train the model for 1000 epochs. In each epoch, perform the following steps:
   - **Forward Pass**: Compute predicted `y` by passing `x` through the model.
   - **Compute and Print Loss**: Calculate and display the loss.
   - **Backward Pass**: Use autograd to compute the gradient of the loss with respect to all Tensors with `requires_grad=True`.
   - **Update Weights**: Apply gradient descent to update weights. Use `torch.no_grad()` to prevent tracking history (and consuming memory).
   - **Manually Zero the Gradients**: Zero the gradients after updating weights to prevent accumulation.
7. **Print Final Values**: Output the final values of `w` and `b`.

## Instructions

1. **Set Up Your Environment**: Ensure you have PyTorch installed in your Python environment.
2. **Implement the Steps**: Follow the requirements above to build and train your linear regression model.
3. **Run the Code**: Execute your code to train the model and observe the results.
4. **Verify Results**: Ensure that the final values of `w` and `b` are close to the expected values.

Happy coding and good luck with your practice!


