# Recommender Systems Class - Project 1: Content Based Hotel Room Recommender
### author: Dominik Mikołajczyk

The tasks given in this project:
- preprocess the data
- bucket important features to reduce the offer space size
- define user features based on reservations
- prepare numerical item features
- code fit and recommend function in content-based recommender class
- tune different ML models to find the best parameters which will improve model's score
- run the final evaluation of each ML model and present the results against the Amazon recommender;s results

## Requirements:
1. Install jupyter:
    <!-- -->
    
        pip install jupyter
        
2. Install other required python libraries:
    <!-- -->
    
        pip install numpy==1.20.1
        pip install pandas==1.2.3
        pip install scikit-learn==0.24.1
        pip install hyperopt==0.2.7
        
* Alternatively if you have Anaconda installed, you can configure enviroment using conda command:
    <!-- -->
    
        conda env create --name rs-class-env -f environment.yml conda activate rs-class-env
        
## Dataset
- [original dataset](https://github.com/ShakinBruno/recommender-systems-project-1/blob/main/hotel_data/hotel_data_original.csv)

![image](https://user-images.githubusercontent.com/71774757/236560653-7c5fa218-282e-4887-9b58-7634e409956e.png)

- [preprocessed dataset](https://github.com/ShakinBruno/recommender-systems-project-1/blob/main/hotel_data/hotel_data_interactions_df.csv)

![image](https://user-images.githubusercontent.com/71774757/236560973-f847f14c-7bfd-4ba7-b917-188cb147c0a3.png)

## Results

![image](https://user-images.githubusercontent.com/71774757/236561393-913e9116-d8b4-41e3-a2fb-5288d5160b72.png)

I was able to beat Amazon Recommender with LinearRegressionCBUIRecommender by 0.002376 in HR@10.
