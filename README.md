# interakt-android
Android Sdk For Android

You’ll need to install Interakt’s latest Android SDK for it to run smoothly on your Android application. Prerequisites:

An Interakt account. You can get started for free!
An Android Application that you are managing.
A few minutes to get you started.

Installation

Step 1
Download Interakt’s latest Andorid SDK.

Step 2
Add the downloaded .aar file as an module in your project.
For this,
Go to file options in your android project and click on new module.
Now import the downloaded .aar in your project and Add as a dependency in your project.


Step 3
To add as a dependency of .aar in your project.
Follow the steps given below :
Go to your project structure, and add .aar module dependency in your project.
Now wait untill the gradle build your project.

Step 4
Now, you can use the interakt sdk in your project.


Step 5
Initialize the sdk.
MyApplication obj = MyApplication.getInstance();’

Call installForApiKey() method with the object of the class and pass the context as a first argument, 
In case of activity pass this else in case of fragment pass getActivity().

In Second Argument pass your Interakt App ID.

obj.installForApiKey(this, "YOUR INTERAKT APP ID");


Step 6.
Add the folllowing code on the button on which you want to show FAQs - 

obj.showFaqs(this,backgroundcolortoshowque,ingridstyle);

Here, the first argument is passed as reference of activity and in second argument we will pass the hexcode color of questions.
You can pass blank string as well in second argument, in that case it will take the default color.
In third argument we will pass boolean value to show the faqs, whether it is to be in grid or in listview.Pass true for gridview else false.

Similarly, If you want to show HELPDESK, add the following code on the button: 

obj.showHelpDesk(this,"#000000");

Here, the first argument is passed as reference of activity and in second argument we will pass the hexcode color of query button to be shown while submitting the ticket.
You can pass blank string as well in second argument, in that case it will take the default color.
