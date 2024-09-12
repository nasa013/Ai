# Recipe Recommendation System API

## Overview

This API offers a recommendation system for recipes based on a hybrid model that combines content-based filtering (using recipe ingredients) and collaborative filtering (using user ratings). It allows users to obtain personalized recommendations and discover similar recipes.

## Features

- **Content-Based Filtering**: Recommends recipes based on similar ingredients.
- **Collaborative Filtering**: Suggests recipes based on user ratings, utilizing the SVD algorithm.
- **Hybrid Recommendations**: Combines content-based and collaborative filtering for a more personalized recommendation.
- **Batch Processing**: Efficiently computes cosine similarity in large datasets.

## Prerequisites

To run this API, you will need:

- Python 3.7+
- Required Python libraries:
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `scipy`
  - `surprise`
- A dataset containing recipe information and user ratings. The dataset should include:
  - `recipe_name`
  - `user_id`
  - `meal_id`
  - `ingredients` (as a list or string)
  - `restaurant`
  - `city`
  - `rating`

## Setup Instructions

1. **Clone the Repository**: Download or clone this repository to your local machine.
   
2. **Install Dependencies**: Install the required Python packages by using the following command:
   
   ```bash
   pip install -r requirements.txt
