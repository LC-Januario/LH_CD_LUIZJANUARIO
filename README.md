# LH_CD_LUIZJANUARIO
Desafio técnico do processo seletivo do programa LightHouse da Indicium


## Setup

To set up the project environment, follow these steps:

1. **Create and activate a conda environment**:

    ```bash
    conda create -n ml python=3.8
    conda activate ml
    ```

2. **Install the required packages**:

    ```bash
    pip install -r requirements.txt
    ```

## Files

- [requirements.txt]: Contains the required packages to run this project.
- [precificacao.ipynb]: Contains the answers to all the questions posed in the challenge and the entire development of an XGBoost model for predicting prices of short-term rental properties, including data extraction, data wrangling, data cleaning, normalization, model training, parameter optimization, model optimization and price prediction.
- [modelo_predição_preço_XGB.pkl]: This is a .pkl file containing the XGBRegressor model.
- [teste_indicium_precificacao.csv]: Contains data used to train and test the model.

## Requirements

The project requires the following packages:

- scikit-learn==1.2.1
- ipykernel==6.20.2
- pandas==1.5.3
- seaborn==0.12.2
- lightgbm==3.3.5
- yellowbrick==1.5
- xgboost==2.1.3

## Usage

1. **Download and install the requirements listed above in your preferred compiler**:

    Make sure all the requirements are met and the enviroment supports python 3.8.

1. **Run the notebooks**:

    Open the notebooks in a Jupyter environment and run the cells in order to perform data wrangling, model training, and prediction. If you wish to import the prediction model into a diferent notebook or environment, you may download the file [modelo_predição_preço_XGB.pkl] and open it using pickle:

   ```bash
   loaded_model = pickle.load(open('modelo_predição_preço_XGB.pkl', 'rb'))

   loaded_model.predict(database)
   ```

## License

This project is licensed under the MIT License.
