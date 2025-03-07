# Recommender Systems Class - Project 1: Content Based Hotel Room Recommender

### Author: Dominik Mikołajczyk

## Project Overview

This project focuses on building a content-based recommender system for hotel rooms. The primary goal is to preprocess data, reduce the dimensionality of the offer space, define user and item features, and implement a recommendation algorithm that can effectively suggest hotel rooms to users based on their preferences and past interactions.

## Tasks

The tasks undertaken in this project include:

- **Data Preprocessing**: Clean and prepare the dataset for analysis.
- **Feature Bucketing**: Bucket important features to reduce the offer space size.
- **User Feature Definition**: Define user features based on reservation history.
- **Item Feature Preparation**: Prepare numerical item features for the recommendation model.
- **Recommender Implementation**: Code the `fit` and `recommend` functions in the content-based recommender class.
- **Model Tuning**: Tune different machine learning models to find the best parameters that improve the model's performance.
- **Evaluation**: Run the final evaluation of each ML model and present the results compared to the Amazon recommender's results.

## Requirements

To run this project, you need to have the following software and libraries installed:

1. **Jupyter Notebook**: For running and interacting with the project notebooks.
    ```bash
    pip install jupyter
    ```

2. **Python Libraries**: Install the required Python libraries using pip.
    ```bash
    pip install numpy==1.20.1
    pip install pandas==1.2.3
    pip install scikit-learn==0.24.1
    pip install hyperopt==0.2.7
    ```

Alternatively, if you have Anaconda installed, you can configure the environment using the conda command:
```bash
conda env create --name rs-class-env -f environment.yml
conda activate rs-class-env
```

## Dataset

The project uses two main datasets:

- **Original Dataset**: [Download here](https://github.com/ShakinBruno/recommender-systems-project-1/blob/main/hotel_data/hotel_data_original.csv)

  ![Original Dataset](https://user-images.githubusercontent.com/71774757/236560653-7c5fa218-282e-4887-9b58-7634e409956e.png)

- **Preprocessed Dataset**: [Download here](https://github.com/ShakinBruno/recommender-systems-project-1/blob/main/hotel_data/hotel_data_interactions_df.csv)

  ![Preprocessed Dataset](https://user-images.githubusercontent.com/71774757/236560973-f847f14c-7bfd-4ba7-b917-188cb147c0a3.png)

## Implementation Details

The project includes several key components:

- **Data Preprocessing Toolkit**: Functions for cleaning and transforming the dataset, such as summing people counts, filtering data, and mapping features to buckets.
- **Recommender Models**: Implementation of various recommender models, including a neural collaborative filtering model (`NeuMFModel`) and a nearest neighbors recommender.
- **Feature Engineering**: Methods for defining and extracting user and item features from the dataset.
- **Evaluation**: Scripts for evaluating the performance of the recommender models using metrics like HR@10.

## Results

The project successfully implemented a content-based recommender system that outperformed the Amazon Recommender. The best-performing model, `LinearRegressionCBUIRecommender`, achieved a higher HR@10 score by 0.002376.

![Results](https://user-images.githubusercontent.com/71774757/236561393-913e9116-d8b4-41e3-a2fb-5288d5160b72.png)

## Conclusion

This project demonstrates the effectiveness of content-based recommendation systems in the context of hotel room recommendations. By leveraging user and item features, the system can provide personalized recommendations that enhance the user experience.
