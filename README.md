# neural_network_charity_analysis

## Overview

For this challenge I created a model that predicts if funding is provided by Alphabet soup to an organization will that organization be successful. To do this I used a CSV that contained over 34,000 previous organizations that were funded and completed created the model around that CSV to predict if an organization will use the money effectively.

## Results

### Data Preprocessing
 - What variable(s) are considered the target(s) for your model?
   * The target for the model is "IS_SUCCESSFUL"
 - What variable(s) are considered to be the features for your model?
   * all columns are features expect for the target column and the two that I dropped/
 - What variable(s) are neither targets nor features, and should be removed from the input data?
   * EIN and NAME were droped as they are neither targets nor features.
 
### Compiling, Training, and Evaluating the Model

 - How many neurons, layers, and activation functions did you select for your neural network model, and why?
   * for the first layer I used 80 neurons and relu activation, for the second layer I used 30 neurons and relu activation and for the outer layer i used sigmoid activation. I used relu to speed up the process.
 - Were you able to achieve the target model performance?
   * No i was not able to hit the 75% target for model performace I achieved 72.8% as shown below. 
   ![base eval](https://github.com/Tyfox1206/neural_network_charity_analysis/blob/main/images/base_eval.PNG)
 - What steps did you take to try and increase model performance?
   * For attempt 1 I reduced the number of applcation types however this did not help achieve the model desired. 
   
   ![attempt1](https://github.com/Tyfox1206/neural_network_charity_analysis/blob/main/images/attempt1_eval.PNG)
   * For attempt 2 I reduced the number of classifications along with the change made in the previous attempt
   
   ![attempt2](https://github.com/Tyfox1206/neural_network_charity_analysis/blob/main/images/attempt2_eval.PNG)
   * For attempt 3 I increaded the in each layer from 80 to 100 and from 30 to 50, along with the changes from pervious attempts.
   
   ![attempt3](https://github.com/Tyfox1206/neural_network_charity_analysis/blob/main/images/attempt3_eval.PNG)

### Summary 

Overall, with this model you will be able to predict if the organization will be success with 72% accuracy. For a recommendation on another model to use I would recommend Random Forest Classifier. For this project it seems the time used to set up all this for 72% accuracy could be achieved much quicker with the random forest classifier as it is easier to set up and will most likely be just as accurate.
