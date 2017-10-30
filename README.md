# Message Processing Application
This is a small message processing (standalone) application for processing sales notification messages.

It is based on the assumption that sales notification come in in JSON format. The application only parses all 
notifications but processes only (first) 50 of them. In actual implementation, the json would probably be received as a
response to an API call, but here it is read from commandline.

##On execution:
1) application initializes stock (read from CSV file provided as commandline argument),
2) parses sales notifications from JSON file (provided as commandline argument), and
3) updates sales register to reflect 50 sales notifications.

##Sample Commandline Arguments:
1) Please adjust path (in the following strings) as per your needs.
2) First argument is stock file: /Users/swati/samples/message-processing-app/src/resources/stock.csv
3) Second and last argument is notifications file: /Users/swati/samples/message-processing-app/src/resources/mixednotifications.json

##Sample Data:
There are five sample data files:
1) stock.csv: This file has stock data listed in there. The data is listed in the order of class (Product) members.
2) notifications.json: This file only has notification messages of Message Type 1.
3) detailednotifications.json: This file only has notification messages of Message Type 2.
4) adjustmentnotifications.json: This file only has notification messages of Message Type 3.
5) mixednotifications.json: This file only has notification messages of all Message Types.

##Next Steps (To-Do list):
1) if time permits, code refactor need to do.
2) need to write the testcases- junit.



