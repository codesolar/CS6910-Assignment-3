# CS6910-Assignment-3
question 1 : It is about encoder decoder model making , the codefile has been added to the  github repo , and the answers of the questions are given in  the wandb report.<br>
question 2 : It is about running sweeps after making the encoder decoder model . The hyperparameter choice strategy is mentioned in the wandb report and the codefile is uploaded in github.<br>
question 3 : This is about making inferences from the available plots (from the sweep run on question 2), The details are written in the wandb report.<br>
question 4 : The best model from sweep is found out and it is trained (after getting the hyperparameter value from wandb sweep) , then it is tested on the test set.Predictions on the test set is uploaded in the github repo.<br>
question 5 : This question is about introducing attention layer in our seq2seq model . The necessery plots are uploaded in report and the codefile is uploaded in github repo.<br>

How to train the model:<br>
One train.ipynb file is attached . <br>
I was running in kaggle , so make sure to upload the aksharantar_sampled zip file in kaggle.<br>
supposedly the user already have aksharanter_sampled zip file, and wnat to run from the terminal , just save this train file in your local machine , open the terminal , go to that directories location with cd command.<br>
then in terminal write 'python3 train.py ' after this write the configurations to train the model .<br>
To run the configurations , the notations are  written below = <br>
        name               <t>    default <br>
-wp       --wandb_project      Assignment 2 <br>
-we       --wandb_entity       cs22m084<br>
-d        --dataset            hin<br>
-es       --embeddingsize      512<br>
-nenl     --number_of_encoder_layers  3<br>
-ndel     --number_of_decoder_layers  1<br>
-hs       --hiddensize                1024<br>
-lr       --learning_rate             0.001<br>
-bt       --beta                      0<br>
-o        --optimizer                 Adam<br>
-bs       --batch_size                128<br>
-bi       --bidirectional             True<br>
-n_iters  --num_iteration             30<br>
-loss     --loss                      cross_entropy<br>
-emn      --encodermodelname          LSTM<br>
-dmn      --decodermodelname          LSTM<br>
-do       --drop_out                  0.2<br>
-attn     --attention                 False<br>
The lines are written in sequence , to run the model of question 4 , just run all the cells , in the 3rd last cell you can see the hyperparameter (eg. embedding size ,...) , put your choice of values there , and in the trainIter too, then run those two cell. the model will automatically run . Then at last run the last cell , it is for evaluating the model on the test dataset , after that it will automatically store the output file in '/kaggle/working' , and one plot will be printed which tells how the model does error with increasing length of word and another plot will be there which will tell how many vowel and consonant it does mistakes on (it is a confusion matrix) . </br>
Link to the wandb report is = https://api.wandb.ai/links/cs22m084/cs8dzyh6
