LabVIEW and Ubidots Example
===========================

In this tutorial we'll explain (1) how to get a value from Ubidots using LabVIEW and (2) how to send a value from LabVIEW.
   
 
Preparing your Ubidots Account
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
Create a Data source called "LabVIEW" and then a variable called "My Variable":

1. As a `logged in user <http://app.ubidots.com/accounts/signin/>`_
   navigate to the "Sources" tab.

2. Create a data source called "My Variable" by clicking
   on the orange button located in the upper right corner of the screen.

3. Click on the created Data Source and then on "Add New Variable".

4. Take note of the variable's ID to which you want to send data. We'll need it later to include in our code.

5. Create a token under "My Profile" tab. We'll need it later for our code.


GET Example
^^^^^^^^^^^
Our GET example will read the last value of the variable from Ubidots. It accepts two inputs: the variable ID and a token generated in your Ubidots account.

Once you run the VI, you'll get the full HTTP response from the server, as well as a parsed numeric value that is extracted from the response. Here's how the code was built.

POST Example
^^^^^^^^^^^^
Our POST example will send an arbitrary value to Ubidots. It accepts three inputs: the variable ID, a token generated in your Ubidots account, and an arbitrary value to send:

Once you run the VI, you'll get the full HTTP response from the serve for debugging purposes. In this case, the value "500" was sent, and it can already be seen in our Ubidots account.

Wrapping up
^^^^^^^^^^^
In this guide we learned how to interact with the Ubidots API using LabVIEW. The possibilities of combining these platfroms are tremendous, given the extensive set of tools in LabVIEW, which includes data acquisition systems, image processing, etc. 
