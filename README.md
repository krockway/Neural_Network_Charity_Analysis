# Neural_Network_Charity_Analysis

## Overview

The purpose of this analysis is to help Alphabet Soup create a neural network model to determine the likelinhood for success when charities seek funding from Alphabet Soup. The model will be built on historical data of  34,000+ organizations that have received funding over the years and their success status.

## Results

### Data Preprocessing

- What variable(s) are considered the target(s) for your model?
  - The target data for this model is the column 'IS_SUCCESSFUL', which indicates whether or not a donation was used effectively or not.

- What variable(s) are considered to be the features for your model?
  - The feature data for this model are the columns 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'INCOME_AMT', and 'SPECIAL_CONSIDERATIONS'.

- What variable(s) are neither targets nor features, and should be removed from the input data?
  - The columns 'EIN' and 'NAME' are neither targets nor features; both of which were dropped from the analysis.

### Compiling, Training, and Evaluating the Model

- What steps did you take to try and increase model performance?
  - I attempted various things to increase the model performance. At first, I tried for a wider model by increasing the number of nodes in each of my 2 layers. In the next attempt, I tried to add depth, by increasing from 2 hidden layers to 8 hidden layers. In my final optimization attempt, I returned to the original settings, but increased the number of epochs from 100 to 1000.

- How many neurons, layers, and activation functions did you select for your neural network model, and why?
  - For my original test, I used 30 nodes in the first layer, 10 nodes in the second layer and ran 100 epochs.
  ![Del2_Summary](https://github.com/krockway/Neural_Network_Charity_Analysis/blob/main/Images/Del2_Summary.png)
  - For my first attempt, I chose to increase the number of nodes from 30 to 300 in the first layer, and 10 to 100 in the second layer. I continued to run 100 epochs.
  ![Del3_Opt1_Summary](https://github.com/krockway/Neural_Network_Charity_Analysis/blob/main/Images/Del3_Opt1_Summary.png)
  - For my second attempt, I chose to keep the increased nodes from Attempt 1, while also increasing the number of hidden layers to 8. Layer 1 kept 300 nodes, while layers 2-8 used 100 nodes. I continued to run 100 epochs.
  ![Del3_Opt2_Summary](https://github.com/krockway/Neural_Network_Charity_Analysis/blob/main/Images/Del3_Opt2_Summary.png)
  - For my third attempt, I went back to the original settings with layer 1 at 30 nodes, layer 2 at 10 nodes, this time increasing the number of epochs from 100 to 1000.
  ![Del3_Opt3_Summary](https://github.com/krockway/Neural_Network_Charity_Analysis/blob/main/Images/Del3_Opt3_Summary.png)

- Were you able to achieve the target model performance?
  - My original model delivered an accuracy of 73.1% and a loss of 55.5%.
  ![Del2](https://github.com/krockway/Neural_Network_Charity_Analysis/blob/main/Images/Del2.png)
  - The first attempt, with added nodes, delivered an accuracy of 73.3% and a loss of 57.3%.
  ![Del3_Opt1](https://github.com/krockway/Neural_Network_Charity_Analysis/blob/main/Images/Del3_Opt1.png)
  - The second attempt, with added nodes & layers, delivered an accuracy of 72.6% and a loss of 57.1%.
  ![Del3_Opt2](https://github.com/krockway/Neural_Network_Charity_Analysis/blob/main/Images/Del3_Opt2.png)
  - The third attempt, with the original nodes and layers, but added epochs, delivered an accuracy of 73.2% and a loss of 57.6%.
 ![Del3_Opt3](https://github.com/krockway/Neural_Network_Charity_Analysis/blob/main/Images/Del3_Opt3.png)
  - Overall, none of my attempts at optimization significantly improved the accuracy of the original model, nor did they reach the targeted 75% accuracy threshold.

## Summary

 Each of my deep learning models were able to reach ~73% accuracy. If I were to continue this process and goal of improving accuracy, I would run another model to combine the additional nodes, layers and number of epochs to see if the combination of all three factors improved the results.

 I would also do further research to bring down the loss amount, which is high.
