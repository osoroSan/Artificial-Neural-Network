# Artificial Neural Network in JavaScript

This repository contains a simple implementation of a neural network in JavaScript, from scratch. No libraries were used. It utilizes the provided `ekko.js` for the neural network, and activation functions (`actFUNC.js`) such as `sigmoid`, `relu`, and `tanh`.

## Contents

1. [Introduction](#introduction)
2. [Usage](#usage)
3. [File Descriptions](#file-descriptions)
4. [Training Script](#training-script)
5. [Contributing](#contributing)
6. [License](#license)

## Introduction

This neural network implementation is designed for flexibility and simplicity in machine learning projects. It supports customizable architectures, activation functions, and training parameters.

## Usage

Ensure you have the necessary modules installed:

Example usage in your project:

## Import necessary modules

const neuralNet = require('./ekko.js');

const { relu, tanh, sigmoid } = require('./actFUNC');

## Create a neural network with specified architecture and parameters

let net = new neuralNet([7, 10, 10, 1], 0.01, sigmoid, sigmoid, false);

## Define training function

const train = (epochs) => {
for (let i = 0; i < epochs; i++) {
console.log(`Iteration ${i + 1}`);
for (let k = 0; k < trainData.length; k++) {
net.train(trainData[0], trainData[1]);
}
}
};

## Train the neural network for 100 epochs
train(100);

## Make predictions on test data
console.log(net.predict(testData[0]));


## File Descriptions

- **ekko.js**: Main neural network implementation.
- **actFUNC.js**: Contains activation functions (e.g., `sigmoid`, `relu`, `tanh`).

## Training Script

In the provided training script (`train.js`), the neural network is instantiated, trained for 100 epochs, and then used to make predictions on test data.

## Contributing

Contributions are welcome! Follow the guidelines in [CONTRIBUTING.md](CONTRIBUTING.md) for more details.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

Remember to replace placeholder text like `trainData` and `testData` with the actual datasets you are using in your project. Feel free to adapt the README to better fit your project structure and details.
