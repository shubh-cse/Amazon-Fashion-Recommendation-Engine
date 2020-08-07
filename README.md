# Amazon Fashion Recommendation Engine

## Background

*Amazon currently uses item-to-item collaborative filtering, which scales to massive data sets and produces high-quality recommendations in real time. This type of filtering matches each of the user's purchased and rated items to similar items, then combines those similar items into a recommendation list for the user.*

## Problem Statement

*In this challenge, we need to recommend similar products (women apparel) to the customers based on brand, color, title, image and others features of the product.*

## Data Set

*You can download the data set from kaggle - https://www.kaggle.com/ajaysh/women-apparel-recommendation-engine-amazoncom*

## Number of Attributes

*Out of these 19 features, we will use only 6 features and image of the product for our analysis:-*

1. asin  ( Amazon standard identification number)
2. brand ( brand to which the product belongs to )
3. color ( Color information of apparel, it can contain many colors as a value ex: red and black stripes ) 
4. product_type_name ( type of the apperal, ex: SHIRT/TSHIRT )
5. medium_image_url  ( url of the image )
6. title ( title of the product )
7. formatted_price ( price of the product)

## Table of Contents

1. Overview of the data
2. Missing data for various features
 2.1 Basic stats for the feature: product_type_name
 2.2 Basic stats for the feature: brand
  2.3 Basic stats for the feature: color
  2.4 Basic stats for the feature: formatted_price
  2.5 Basic stats for the feature: title
3. Remove near duplicate items
  3.1 Understand about duplicates
  3.2 Remove duplicates
4. Text pre-processing
5. Text based product similarity
  5.1 Bag of Words (BoW) on product titles
  5.2 TF-IDF based product similarity
  5.3 IDF based product similarity
6. Text Semantics based product similarity
  6.1 Average Word2Vec product similarity
  6.2 IDF weighted Word2Vec for product similarity
  6.3 Weighted similarity using Brand and Color
  
## A glimpse of the Recommendation Engine

![recommendation_1](https://user-images.githubusercontent.com/68144553/89631864-fee49300-d8be-11ea-988f-32ec4e318918.JPG)
![recommendation_2](https://user-images.githubusercontent.com/68144553/89631872-00ae5680-d8bf-11ea-8e4b-ae2492eb5650.JPG)
![recommendation_3](https://user-images.githubusercontent.com/68144553/89631876-0146ed00-d8bf-11ea-8b8b-e8ba4df5d4e9.JPG)
![recommendation_4](https://user-images.githubusercontent.com/68144553/89631882-02781a00-d8bf-11ea-894c-609e48abbc17.JPG)
![recommendation_5](https://user-images.githubusercontent.com/68144553/89631887-0310b080-d8bf-11ea-88df-7d353b7879be.JPG)
