# CS6910-Assignment-3
question 1 : It is about encoder decoder model making , the codefile has been added to the  github repo , and the answers of the questions are given in  the wandb report.
question 2 : It is about running sweeps after making the encoder decoder model . The hyperparameter choice strategy is mentioned in the wandb report and the codefile is uploaded in github.
question 3 : This is about making inferences from the available plots (from the sweep run on question 2), The details are written in the wandb report.
question 4 : The best model from sweep is found out and it is trained (after getting the hyperparameter value from wandb sweep) , then it is tested on the test set.Predictions on the test set is uploaded in the github repo.
question 5 : This question is about introducing attention layer in our seq2seq model . The necessery plots are uploaded in report and the codefile is uploaded in github repo.

How to train the model:
I was running in kaggle , so make sure to upload the aksharantar_sampled zip file in kaggle.
The lines are written in sequence , to run the model of question 4 , just run all the cells , in the 3rd last cell you can see the hyperparameter (eg. embedding size ,...) , put your choice of values there , and in the trainIter too, then run those two cell. the model will automatically run . Then at last run the last cell , it is for evaluating the model on the test dataset , after that it will automatically store the output file in '/kaggle/working' , and one plot will be printed which tells how the model does error with increasing length of word and another plot will be there which will tell how many vowel and consonant it does mistakes on (it is a confusion matrix)
