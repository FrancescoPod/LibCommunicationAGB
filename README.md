# Introduction
This is the library of Arduino Gui Builder program.
You will be albe to create small GUI for your arduino easily without coding.
* Download the zip file, extract the folder and put it in the libraries of Arduino IDE.
* There are 3 projects as examples where you can learn how to use the library.
* This library is necessary to handle the communication between the board and your pc.
# How to use the library
Threre are 3 different objects:
* MultiSender: it can send multiple data to your pc. It requires two arguments: 1) they array of formats 2) the length of the array.
* SingleSender: it can send only one data to the pc. it requires only one argument: the format.
* Receiver: it can read a value form the pc through the Serial Monitor and return it as a string.
# What is a format?
The "format" is simply a way to organise a string in order to let the Arduino GUI Builder know where to put this value.
Example, if you write in Arduino (after you have added this library) CodeA it will correspond to A!x!A. The library will parse this format and it will become: A!myVal!A.
There are 21 different formats. They follow the italian alphabet.
CodeA, CodeB, CodeC, CodeD, CodeE...
# Others methods
* If you want to check if there are errors (because the communication may not work) you can use the method .debug(); It will display on the Serial Monitor the state of  the object it can be called on a MultiSender, SingleSender and Receiver.
* When you have to add the data to a SingleSender or to a MultiSender you have to write .addData() it will take a string (format) if it is a SingleSender, otherwise it will take an array of string (array of formats).
* When you want to send to the pc the value that you have just added to the senders you can call .flush().
* When you want to read what the pc has just sent to the board, write .read() on a Receiver, it will return the message as a string.
# Info
For any questions you can watch the documentation on the website.
You can contatc me at: francesco.podesta03@gmail.com
I'm Francesco Podestà and I am a student of high school.
# Have Fun!!

