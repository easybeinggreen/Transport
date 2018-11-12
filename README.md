# Transport

Hi mark,

My first github contribtuion!

Very grateful if you could take a look through when you have a moment and if we could discuss some of the following points when we speak.  Monday to Thursday is good for me can come to you in person or via Zoom. I have set up a Zoom account,

The notebooks are roughly as follows:

  1 Data exploration uses the initial training data AND tha later, merged comnined training and test data to get a general picture.
  
  2 Preparing uber data: some work done on the uber-generated csv then leg a to b and leg b to c combined to create new df here
  
  3 Merging the Uber and mobi data, Separating train and test, creating validation set, running initial random forests and tweaking max_leaf nodes
  
  4 Forest Models: Introducing graphing of the validation set to identify minima and feed into model. Introducing gridsearch cv getting 3.3 on validation, 3.9 on test
  
  5 xgboost following similar pattern of graphing validation sets and using gridsearch. Again getting 3.6 on validation and 4.11 on test
  
I never did better than running an untrained Randomm Forest without Uber data! Giving me 3.7 on test data. My position is now slipping
  
  Questions / topics for discussion
  
Even though I am performing reasonably well on the validation data this is not translating into a score on test data, presumably due to overfitting. How to solve this? EG in Notebook 4 model 5,7,8. Is it overfitting as I am not using test_v_y in building model (other than when i am playing with graphs)

    
Is there a way of manipulating training set to more closely match the structure of the test set eg proportion of bus vs shuttle
    
I think the data from Uber is not very helpful in the form I have it, the feature selection shows the model uses it but scores are worse when it is included so I need to either look again at how i generated it, use fewer indicators. It may be GARBAGE IN. How should I best use the feature seleciton info in notebook 5. Just because its important dosn;t mean its helping right?
   
How should I create the final model to run on test data? SHould I use the exact model I have been training on the validation test set and just fit that to the full test set? OR Should I run a cross validation on the full training set and use the best result of that.... or a combination of both?

Comments on general approach eg naming of models, managing notebooks, version control, code, use of programming techniques eg loops and formulss, notes etc would be very helpful. How do you keep track of results and log them? Is there a good way?

What is the next step?

SHould I go back and try and improve the quality if the data from Uber?

Should I venture into using Lasso/ElasticNet/Ridge to sharpen features.

Are there aspects of tuning I have not used or not used correctly


Other thoughts...

Am keen to get stuck in to reading papers as you suggest. Where would you suggest I start? I had a look at Breimann 2001 on Random Forests, is that the kind of thing you had in mind?

Looking forward to speaking when you can make it. So many questions

I cannot thank you enough for your input

With very best wishes

Paul
