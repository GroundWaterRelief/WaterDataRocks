# WaterDataRocks
Scripts related to the WaterDataRocks App

This memorandum is here to provide a guidance on how to link client/external database (EXT DB) to WaterDataRocks Database (WDR DB).

Objective: Obtain the data stored in WDR DB via a Python request.
Groundwater Relief provides you with endpoints allowing you to obtain the data stored in WDR DB.

What is an endpoint: An endpoint is a specific location in a computer network where data can be sent or received. It is an interface that allows communication between different systems or components within a network. In the context of web development and APIs, an endpoint is a URL that represents a specific resource or service, which can be accessed by making an HTTP request (e.g., GET, POST, PUT, DELETE). When a client sends a request to an endpoint, the server processes the request and returns a response, usually in the form of data.
GET request: Groundwater Relief allows you to make a GET request, which allow to GET the data from WDR DB. 

What is provided by GWR: 
•	This memorandum,
•	2 endpoints (so 2 URLs):
  o	One for all monitoring values
  o	One for all monitoring points
•	The GWR ACCESS CODE that allow you to fetch the data corresponding to the data you want. 
•	The request script in Python as an HTML. It can be used by copy pasting and running the python requests in your workflow:
  o	As a courtesy, it includes an example of the merge to be done to link the 2 tables (monitoring values and monitoring points) (PLEASE DO NOT TAKE THIS AS THE CORRECT WAY AND MERGE AS YOU NEED). 
  o	It also includes examples of function to be called to manipulate the data once extracted from the WDR DB.

Once the GET data from the WDR DB, it is up to the client to: 
•	Manipulate the data to map them to the client database (it can be done via a python script for instance),
•	Insert the data to the client database,
•	Export the data in a different format if deemed necessary.
