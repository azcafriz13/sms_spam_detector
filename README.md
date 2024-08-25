# Challenge Module 21
## SMS Spam Detector: An ASU AIML Challenge by CA Frisby

### Overview
Import a .csv file with "spam" and "ham" classifications for SMS text messages.
Use this already classified data to build aan SVC model to evaluate other SMS
text.  Use a Gradio Interface application to allow user input of new SMS text
for classification using the model. 

References:  Starter code was provided by ASU AIML. Additional references are
cited within the code.
             
### Part 1:  Create the SMS Classification Function

The features variable is set equal to the text message column of the DataFrame.
The target variable is set equal to the "label" column of the DataFrame.
The data is split into training and testing sets, and the test_size is set to 33%.
A Pipeline is built using the TfidfVectorizer and LinearSVC to transform the test 
set and compare it to the training set.

The model is fitted to the transformed training data and the model is returned.

The SMSSpamCollection.csv is read into a DataFrame.

The DataFrame is passed to the sms_classification function and the result is set 
equal to the "text_clf" variable.

### Part 2:  Create the SMS Prediction Function
A new variable holds the prediction of a new text.
A conditional statement determines if the text message is "ham" or “spam”.
The conditional returns a message if the text is “ham” or “spam”.

### Part 3: Create the Gradio Interface Application
A Gradio Interface application is created with three parameters for the 
“function”, “outputs”, and “inputs”.
The “outputs” parameter is a textbox that contains a label to let the user know 
what to type in the box.
The “inputs” parameter is a textbox that contains a label to let the user know 
that the prediction will be displayed in the textbox.
The Interface application can be shared with other users with a public URL.
For this version of the code, the public URL is commented out.  This triggered
an antivirus response.  

Some SMS messages are included in comments for testing after the gradio interface.




