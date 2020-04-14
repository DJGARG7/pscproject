### *How to run the CHATBOT*

1) We have used `tensorflow` in the backend so you will have to run it in python 3.6 environment (since tensorflow is not availible in python 3.7 yet).
2) Install keras, nltk, json, pickle and tensorflow in the 3.6 environment.
3) Download wordnet and punkt by nltk.download('wordnet') and nltk.download('punkt')
4) Run the file `python train_chatbot.py` to train the model from 'intents.json' to create 3 layer neural network
5) Now run the file named `python chatgui.py` and the chatbot will be on your screen and u can start interacting with it.


<img src="https://github.com/DJGARG7/pscproject/blob/master/test.gif">

### *Components of GUI*
The GUI components have been made by making the use of tkinter module
*base = Tk()*
#### 1) The Base box
It is titled 'Hello', is not resizable and has the fixed geometry 400 x 500
*base.title(), base.geometry(), base.resizable()*
#### 2) The Chatlog 
It has the fixed height 8 and width 50
*Chatlog = Text(base,...)*
#### 3) The scrollbar
It is used for scrolling the chatlog
*scrollbar = Scrollbar(base,command=ChatLog.yview,...)*
#### 4) Entry Box
It is a text box used to take input entry from the user. The default font is set to Arial.
*EntryBox = Text(base,.,font='Arial',.)*
#### 5) The Send button
It is used to submit/send the text inserted in the Entry box. On clicking on this button, the text in entry box is cleared to take new input from user.
*SendButton = Button(base,...,command= send,...)*
