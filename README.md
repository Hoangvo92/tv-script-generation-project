# tv-script-generation-project
This is a project that generates a fake script from a provided TV script by using RNNs. 
The provided dataset is the Seinfeld dataset of scripts from 9 seasons.
The neutral network that I built generate a new, "fake" tv script.


## Basic knowledge in this project

In this project, I used lessons from Udacity about deep learning in training data:
   *Recurrent Neutral Networks (RNNs)
   *Long-short term Memory Networks (LSTMs)
   *Hyperparameters
   *Embedding and Word2Vec
   

## Basic Installation

Please read the READMEBasicInstallation.md and requirements.txt before continue. You need to set up your environment with anaconda, jupyter notebook, python, and many necessary packages before running the project with new dataset.
To run the project, you must have a GPU training environment.


## Clone the Project from github

In your device, you should choose a suitable directory, activate command prompt, and go to that directory.
You will run these commands on command prompt.
   ...
   git clone https://github.com/Hoangvo92/tv-script-generation-project.git
   ...
   ...
   cd tv-script-generation-project
   ...
   
   
## Run the project in your GPU environment

First, in the directory tv-script-generation-project, run the command:
   ...
   jupyter notebook
   ...
In the browser being support with GPU, open the file dlnd_tv_script_generation.ipynb

You will notice the first cell in the ipynb file:
   ...     
   import helper
   data_dir = './data/Seinfeld_Scripts.txt'
   text = helper.load_data(data_dir)
    ...

if you have a new dataset, you can change the default dataset Seinfeld_Scripts.txt. Notice: the dataset must be a script similar to this:

 "
 jerry: do you know what this is all about? do you know, why were here? to be out, this is out...and out is one of the single most enjoyable experiences of life. people...did you ever hear people talking about we should go out? this is what theyre talking about...this whole thing, were all out now, no one is home. not one person here is home, were all out! there are people trying to find us, they dont know where we are. (on an imaginary phone) did you ring?, i cant find him. where did he go? he didnt tell me where he was going. he must have gone out. you wanna go out you get ready, you pick out the clothes, right? you take the shower, you get all ready, get the cash, get your friends, the car, the spot, the reservation...then youre standing around, what do you do? you go we gotta be getting back. once youre out, you wanna get back! you wanna go to sleep, you wanna get up, you wanna go out again tomorrow, right? where ever you are in life, its my feeling, youve gotta go. 

jerry: (pointing at georges shirt) see, to me, that button is in the worst possible spot. the second button literally makes or breaks the shirt, look at it. its too high! its in no-mans-land. you look like you live with your mother. 

george: are you through? 

jerry: you do of course try on, when you buy? 

george: yes, it was purple, i liked it, i dont actually recall considering the buttons. 

 "
 If you change the format, then you should make sure that it is uniform as dialogs of conversations. Try to have a .txt file of more than 1MB, so the training RNN can train the data.
 
 Next, you will run all cells inside the notebook. The processing will take time.
 If you are unclear, then there are more instruction in the ipynb file.
 The fake script will be nonsensical unless there is a big dataset and a lot of training time.
