# Test case: Not Fall Detection device
## Test Case ID: 
## Description
This test shall show when the elder performs normal movement, there will not notify on display.
## Procedure
1. Connect boart to computer
2. Test the movement by holding the board and moving slowly.
## Test Device
Check movement accuracy
## Expected Result
Display shall not show Fall detected because display shall notify only when the elder fall.


# Test case: Fall Detection
## Test Case ID: 
## Description
Examine the fall of the elderly, which will be detected when the elderly fall.
## Procedure
1. Connect the board to the computer to test for fall.
2. Test by releasing the board quickly to simulate the fall.
## Test Device
Check movement accuracy
## Expected Result
Fall detected was a show in display .


# Test case: Test MQTT
## Test Case ID: 
## Description
Show that MQTT can connect on NETPIE. 
## Procedure
1. Connect board and MQTT server together.
## Test Device
Send Fall Detection message to MQTT.
## Expected Result
Show status connected on NETPIE.


# Test Case : Server Data Sorting
## Test Case ID : 001
## Description
This test shall show whether the application handle the incoming MQTT messages correctly with their corresponding database column
## Procedure
1. Publish a test MQTT messages
2. Change MQTT topics
3. Verify data in the database
## Test Data
Various MQTT topics
## Expected Result
App shall assigned the payload to the database column according to the received MQTT topic


# Test Case : Get Request endpoint
## Test Case ID : 001
## Description
In order to summarize the database, the server needs to provide the correct response for the request
## Procedure
1. Perform a GET request to the application
2. Verify the json response
## Test Data
Postman (Get request)
## Expected Result
Postman should show only fall people’s name and the time when people fall
