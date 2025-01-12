# NLPrescue: Intelligent Disaster Tweet Analysis System

A machine learning project that uses Natural Language Processing (NLP) to identify and classify real disaster-related tweets from non-disaster tweets.

## Overview

TweetAlert is an intelligent system that helps emergency responders and disaster management teams quickly identify genuine disaster-related social media content. Using advanced machine learning techniques, it differentiates between tweets about actual emergencies (e.g., "Forest fire spreading near downtown!") and non-emergency tweets using similar language (e.g., "This new album is fire!").

## Project Structure

```
.
├── .github/             # GitHub Actions workflows
├── ML/                  # Core ML implementation
│   ├── data/           # Training and test datasets
│   ├── dataset/        # Data loading and processing
│   ├── helper_functions/# Utility functions
│   ├── modelling/      # Model implementations
│   └── predictions/    # Model outputs
├── tests/              # Test suite
└── wandb/             # Weights & Biases logging
```

## Features

- Binary classification of tweets (disaster vs non-disaster)
- PyTorch-based implementation
- Multiple model architectures
- Weights & Biases integration for experiment tracking
- Comprehensive test coverage
- GPU acceleration support

## Requirements

- Python 3.7+
- PyTorch
- torchvision
- torchtext
- pandas
- numpy
- scikit-learn
- wandb
- matplotlib
- tqdm

## Installation

1. Clone the repository

```bash
git clone https://github.com/Programmer-RD-AI/NLP-Disaster-Tweets.git
```

2. Install dependencies

```bash
pip install -r requirements.txt
```

## Usage

To train the model:

```
python run.py
```

Monitor training progress in the Weights & Biases dashboard.

## Dataset

The project uses two main datasets:

- train.csv: Labeled tweets for training
- test.csv: Unlabeled tweets for prediction

Labels:

- 1: Real disaster
- 0: Not a real disaster

## Contributing

1. Fork the repository
2. Create a feature branch
3. Commit changes
4. Push to the branch
5. Open a pull request

## License

This project is licensed under the Apache License 2.0 - see the LICENSE file for details.
