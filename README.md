# <p align='center'>IT496 - Introduction to Data Mining</p>
**Course Project**: 2 <br/>
**Lab Group**: T06<br />
**Dataset**: IP Network Traffic Flows


## **Introduction**: 
The given dataset is about the network flow statistics collected by performing packet captures over 6 days of April 2017. It contains information about an IP flow. An Ip flow consists of all traffic that belongs to the same communication context, that is the same connection between two network devices. Information about a sequence of packets is included. Datafields like Source IP, destination IP, source and destination port addresses, protocols used, interarrival times(time gap between two packets), etc are stored and are collected through CICIFlowmeter app.
* The dataset is of dimensions $35,77,296\times87$. There are $35,77,296$ instances of data and there are $87$ columns in each instance.<br/>
A summary of all the columns present in the dataset:<br/>
1)Flow Id: A unique Id assigned to each of the IP flow captured<br/>
**Attribute Type** : Nominal , **Null count**:0
**Unique value count**: 1522957
