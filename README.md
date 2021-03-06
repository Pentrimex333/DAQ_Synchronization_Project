# DAQ_Synchronization_Project
The codes included in here were primarily coded by me during my time working in the Anschutz Medical Campus's Optogenetic Neural Engineering Core. While I cannot claim entire ownership of these codes (in particular the Arduino barcode generator), I did make very significant contributions to all of them.

These codes are used to align data collected from two different DAQ (data acquisition) systems. This is needed because when using two or more DAQ systems to collect data, the difference in DAQ starting times and frequency of data collection can lead to difficulty in aligning that data to one another. These codes are designed to produce a synchronizing signal (in our instance, a 32-bit "barcode") which is sent at regular intervals through an Arduino board to these different DAQ systems. We then use the signal in both cases to match the starting point and frequencies of the data produced, and finally merge them into a single, easy-to-use dataset that is completely synchronized across time.

![Data Flow Diagram](flowdiagram.drawio.png)
