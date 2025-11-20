Contents: A guide on how to open, run, and view the results of the accompanying .json flow file.
1. Prerequisites
For the flow to run correctly, you must have Node-RED installed on your machine.

Essential Requirement: This flow uses the Dashboard user interface. Please ensure you have the following package installed in Node-RED:

node-red-dashboard

(To install: Go to the Menu > Manage Palette > "Install" tab > Search for node-red-dashboard and install it.)


2. How to Open and Import the JSON Flow:
   
Please follow these steps to import the accompanying .json file into your Node-RED environment:

Open the Node-RED Editor: Go to your browser and open the default address: http://localhost:1880.

Access the Import Menu: Click on the Main Menu (the three horizontal lines in the upper right corner).

Select "Import": From the dropdown menu, choose "Import".

Upload the File: Select "Select file to import" (or "paste your flow here"), and upload the Green Box .json file.

Choose Import Location: Ensure you select "New Flow" when importing.

Click "Deploy": After the flow appears in the editor, click the red "Deploy" button in the upper right corner to activate the flow.



3. How to Run and View Results (The Dashboard):

This flow is designed to simulate the processing of racing data and display the deterministic decision of the Green Box system.

3.1 Viewing Results on the Dashboard
To view the outputs of the Deterministic Decision Engine:

Open the Dashboard: In your browser, open the standard Node-RED Dashboard path:
http://localhost:1880/ui
What to Expect: You will find a dashboard displaying the following metrics and visual indicators:
(Gauge):
Green (Healthy): Performance is within the normal range (Optimal).
 Yellow (Caution): Performance is approaching the failure threshold. Immediate monitoring is required.
 Red (Critical/Imminent Failure): The Anomaly Score has exceeded the threshold. The Closed-Loop Logistics Action is triggered



 3.2 Running the Simulation:
Automatic Start: If the flow is receiving data from a simulation source (such as a time-based Inject node), processing will start automatically after you click Deploy.

Manual Start (If Required): If manual triggering is needed, please click the "Inject" node (usually found at the start of the flow) to begin sending data.
