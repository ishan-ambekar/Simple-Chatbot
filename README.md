# Simple-Chatbot
A simple chatbot based on reddit comments.

This Chatbot has been trained on reddit comments.

STEPS to proceed:
1.Download the reddit comments dumps either using torrent or from this website (http://files.pushshift.io/reddit/comments/)

2.Execute the chatbot_database_data script.(Change the paths according to the location of your dataset)

3.Execute the chatbot_training_data script. The data will be seperated into test and train files.

4.Install the nmt-chatbot repository(https://github.com/daniel-kukiela/nmt-chatbot, Based on Neural Machine Translation). Make sure all the requirements are satisfied.

5.Place training data inside "new_data" folder (train.(from|to), tst2013.(from|to), tst2013(from|to)). That is, the files created after step 3.

6.Change your directory to setup inside nmt-chatbot. Edit the settings.py file according to your liking. (For eg - increase the vocab size if your gpu is great)

7.Run setup/prepare_data.py

8.Move out of setup directory.

9.Run train.py

This will start the training process. Depending on your gpu, the training time will fluctuate a bit.

For results:

1.Execute the inference.py script.(in nmt-chatbot folder)

The more data you use, the better the model will be

