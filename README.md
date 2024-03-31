# ScikitPipe: Streamlined Machine Learning Pipelines with Scikit-learn

ScikitPipe is a Python project designed to simplify the process of building and deploying machine learning classifiers using Scikit-learn. This project allows users to define their data preparation steps and visualization preferences in a JSON file, which is then used to construct a Scikit-learn pipeline.

## Features

- **Configurable Pipeline**: Define data preprocessing steps and classifier configurations in a JSON file.
- **Efficient Workflow**: Streamline the machine learning workflow from data preparation to model evaluation.
- **Visualization Options**: Easily include visualizations such as confusion matrices for better understanding of model performance.
- **Extensible**: Customize and extend functionalities as per project requirements.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/vinicius-viude-portfolio/scikit-pipe.git
   cd ScikitPipe
   pip install -r requirements.txt

## Usage

1. Create a JSON file (config.json) to define your data preprocessing steps and visualization preferences. Example configuration:

    ```json
    {
    "data_preparation": {
        "imputer": {
            "strategy": "mean"
        },
        "scaler": "standard"
    },
    "classifier": {
        "algorithm": "RandomForest",
        "parameters": {
            "n_estimators": 100,
            "max_depth": 5
        }
    },
    "visualization": {
        "confusion_matrix": true
    }
    }

2. Run the main.py script with the path to your configuration file:

    ```bash
    python main.py --config config.json

## Contributors

- Vinicius De Martin Viude

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
