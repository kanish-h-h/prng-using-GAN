## Project Sturcture

```
prng_project/
│
├── prng/                   # Main package
│   ├── __init__.py         # Marks the directory as a package
│   ├── generator.py        # GAN generator logic
│   ├── discriminator.py    # GAN discriminator logic
│   ├── training.py         # Training pipeline for GAN
│   ├── evaluation.py       # Evaluate the quality of generated random numbers
│   ├── utils.py            # Helper functions (e.g., data preprocessing, metrics)
│
├── data/                   # Directory for datasets
│   ├── raw/                # Raw datasets
│   ├── processed/          # Preprocessed datasets
│
├── tests/                  # Unit and integration tests
│   ├── __init__.py
│   ├── test_generator.py   # Tests for the generator
│   ├── test_discriminator.py # Tests for the discriminator
│   ├── test_training.py    # Tests for the training pipeline
│   ├── test_utils.py       # Tests for utility functions
│
├── scripts/                # Scripts for experiments or training
│   ├── train.py            # Script to run GAN training
│   ├── evaluate.py         # Script to evaluate GAN performance
│
├── notebooks/              # Jupyter notebooks for exploration and visualization
│   ├── exploration.ipynb   # Initial GAN architecture and experimentation
│
├── models/                 # Directory to save trained models
│   ├── gan_generator.pt    # Saved generator model
│   ├── gan_discriminator.pt # Saved discriminator model
│
├── logs/                   # Logs for training and evaluation
│   ├── training.log        # Training logs
│   ├── evaluation.log      # Evaluation logs
│
├── requirements.txt        # Python dependencies
├── setup.py                # Setup script for packaging
├── README.md               # Project overview and usage instructions
├── .gitignore              # Git ignore file
├── LICENSE                 # License file (optional)
└── config.yaml             # Configuration file for hyperparameters
```
---

### Key Components Explained
1. Main Package (prng/):
    - Contains the core implementation of your PRNG using GANs.
    - Modules for the generator, discriminator, training pipeline, and utility functions ensure modularity.

2. Data Directory (data/):
    - Stores raw and processed datasets. Helps in keeping the data organized.

3. Tests (tests/):
    - Unit and integration tests to validate the implementation.
    - Helps in ensuring reliability.

4. Scripts (scripts/):
    - Standalone scripts for training and evaluating the model. Useful for production and experimentation.

5. Notebooks (notebooks/):
    - Use Jupyter notebooks for exploring and testing ideas before integrating them into the main codebase.

6. Models (models/):
    - Store trained GAN models, making it easy to reload them for evaluation or deployment.

7. Logs (logs/):
    - Logs for tracking the training and evaluation process, helping with debugging and performance tracking.

8. Dependencies (requirements.txt):
    - List all dependencies required for the project to ensure consistent environments.

9. Setup Script (setup.py):
    - Package your project so others can easily install it using pip.

10. Configuration (config.yaml):
    - Centralized configuration for hyperparameters and settings, making the code flexible.

11. Documentation (README.md):
    - Provide an overview, installation steps, usage instructions, and examples.
