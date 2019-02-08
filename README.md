 

# Chatbot using Python and Tensorflow 

## A fourth-year first semester mid-term project report submitted for partial fulfilment of the requirements for COMP 484. 

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
   [Sqlite]()
   
   ### Nueral Machine Translator(N.M.T) Model
   
   To train the model, we have used Tensorflow's Seq2Seq NMT Model. Originally, this model was used for text translation from English to French Language. We've tweaked this model to output English Language.
    
    
    

  
