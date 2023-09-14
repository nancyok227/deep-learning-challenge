* Data Preprocessing
    1. * The target variable is the 'IS_SUCCESSFUL' column from application_df.
    2. * The feature variables are every other column from application_df --> this was defined by dropping the 'IS_SUCCESSFUL' column from the original dataframe.
    3. * The 'EIN' and 'NAME' columns were dropped/removed, because they were neither targets nor features for the dataset.

* Compiling, Training, and Evaluating the Model
    4. * In the first attempt, I used 80 nodes for the first hidden layer and 30 nodes for the second hidden layer -- these were just random guesses. 
       * For the second attempt, I used 10 nodes for the first hidden layer and 8 nodes for the second hidden layer -- also these were just random guesses to check if better optimization rate could be achieved for the model.
       * Lastly, 3 layers were tried on the model with nodes 90, 40, and 10 for the first, second, and third layers respectively and the epochs was increased from 100 to 120 for the third attempt.

    5. I was not able to achieve the 75% model accuracy target.

    6. I added more layers at some point, removed more columns, added additional hidden nodes, and increased the epochs in one of the attempts, all in an attempt to achieve higher model accuracy. 
    

* Summary
In terms of forecasting the classification problem, the deep learning model was approximately 73% accurate. Higher prediction accuracy would probably result from using a model with more input-output correlation. This might be accomplished by performing additional data cleaning up front, employing a model with alternative activation functions, and iterating until a greater level of accuracy is attained. 