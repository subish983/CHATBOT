 

# Chatbot using Python and Tensorflow 

## A fourth-year first semester mid-term project report submitted for partial fulfilment of the requirements for COMP 484. 
   Project Supervisor: Dr. Bal Krishna Bal, H.O.D DoCSE K.U. </br>
   

### Background

   The chatbot is a computer program or an artificial intelligence which conducts a conversation via auditory or textual methods. 
     
### Objectives
  + To create a chatbot that can interact and have a conversation with its user.
  + To use the language translator’s sequence to sequence model to create an interactive bot.
  + To create an online bot that could be used as a conversational program in online game streaming websites.

### Dataset Source

  For the dataset used in the model, we used the readily available dump data of 1.7 Billion Reddit Comments. We trimmed down the data to only a month of data of Jan 2015.
  
  [*1.7 Billion Reddit Comments Dataset*](https://www.reddit.com/r/datasets/comments/3bxlg7/i_have_every_publicly_available_reddit_comment/?st=j9udbxta&sh=69e4fee7) 
  
  ### Database Used
  
   We filtered down the reddit comments from two parameters:
   * their score(i.e. only accepted the comments with a score >= 2)
   * comment length (i.e. number of words >1 and < 50)
   
   We then stored this data in sqlite database for our model. 
   [Sqlite](https://sqlitebrowser.org/)
   
   ### Nueral Machine Translator(N.M.T) Model
   
   To train the model, we have used Tensorflow's Seq2Seq NMT Model. Originally, this model was used for text translation from English to French Language. We've tweaked this model to output English Language.
   
   [Link to our NMT Model](https://drive.google.com/file/d/1pyeu4B4j_xsl0jGCMcJKf-cJ5Eqd268P/view?fbclid=IwAR0_fcEzyJurOhB6M8NYzrg7YiaKlf13MSUuR0P_W0jCOQOUUJAwnFXJXJg)
   </br>
  **Note**
    </br>
  * Our model is under the folder named 'model'.
  * All the output files after training the model have been saved in the 'model' folder as 'translate.ckpt' files.
  * The training and testing data files are inside the 'new_data' folder.
  
  ### Output
  
  * The interface for the bot can be accessed through the 'modded-inference.py' file.
    
  ### Results
  
   Made an interactive bot having the following params:
  * Training Steps: 30, 000
  * Learning Rate: 0.001
  * Words Per Second Learnt: 11.52K
  * Perplexity Value: 38.95
  * Gradient Noise: 5.90
  * Bleu Value: 2.78
  
  #### Calculating Accuracy
   
   Taking Google Translator's Bleu Value as a Reference Value :
  * Google Translator's Bleu Value: 3.694
  * Our  Model's Bleu Value: 2.78
  * Accuracy of Our model based on Bleu Value = 75%
  
    
    

  
