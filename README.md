# Automatic-billing-system
To integrate the charge from the optical microscope, the advanced optical microscope and the electronic microscope, I designed this system to automatically sort bills to each project investigator and generate monthly and yearly data.

#Instructions 

A. Install
1.	Download the knwf file.
2.	Install KNIME in your PC.
3.	Import the download knwf file as a workflow under KNIME environment.

B. Automatic sorting
1.	Reset this KNIME workflow.
2.	Configure the node “Import C” to the working log of confocal microscopes.
3.	Configure the node “Import MC” to the working log of microscopes.
4.	Configure the node “Import EM” to the working log of electron microscopes.
5.	Configure the node “Create File Name” to the folder where stores the sorted bills.
6.	Execute the node 7 to start automatically bill sorting in the specified folder.

C. Monthly collection
1.	Set file path from the exported folder where contains the sorted bills in node 72.
2.	Rename the file name to collect the monthly data in node 77.
3.	Execute node 77.

D. Yearly collection
1.	Configure the node “Import monthly sum” to the file created by node 77.
2.	Configure the node “Import Sum” to the file carrying the previous collection.
3.	Rename the output file name in node 84.
4.	Execute node 84.
#Feedback
1.	Made changes to the layout templates or some other part of the code? Fork this repository, make your changes, and send a pull request.

