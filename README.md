# sfguide-getting-started-with-automl-openfe-and-autogluon

## Overview
This example uses a feature engineering package (OpenFE) to create features (column interactions, column transformations) from a Snowflake table.

The derived features are then saved as a FeatureView in the FeatureStore. Once saved both Snowflake.ML or any Open Source package (AutoGluon) can be used to train a model.

Features that are derived are saved as well as the formula used to create it, as a comment for the feature. This enables a user to understand how the feature was created. This can be very important in industries that are regulated as the feature might need to be explained and understood before deployment.

As part of this example, several notebooks show how to train using the derived features:

AutoGluon uses AutoML to create a model.
Snowflake.ML, is used to create XGBoost model
AutoGluon Time Series, as an example of using AutoMl for time series problems.
Regardless of the training notebook / package used, they can all be deployed using Snowpark Container Services, as such all the notebooks contain code to register the model, create and deploy the model.

Lastly the notebooks contain examples of how to call the models predict function and a separate notebook shows how to call the model predict remotely (outside of Snowflake) and return prediction using either Snowpark or a pure HTTP request.

## Step-by-Step Guide
For prerequisites, environment setup, step-by-step guide and instructions, please refer to the [QuickStart Guide](https://quickstarts.snowflake.com/guide/getting-started-with-automl-openfe-and-autogluon/index.html).
