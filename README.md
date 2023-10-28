# <p align='center'>IT496 - Introduction to Data Mining</p>
**Course Project**: 2 <br/>
**Lab Group**: T06<br />
**Dataset**: IP Network Traffic Flows


## **Introduction**: 
The given dataset is about the network flow statistics collected by performing packet captures over 6 days of April 2017. It contains information about an IP flow. An Ip flow consists of all traffic that belongs to the same communication context, that is the same connection between two network devices. Information about a sequence of packets is included. Datafields like Source IP, destination IP, source and destination port addresses, protocols used, interarrival times(time gap between two packets), etc are stored and are collected through CICIFlowmeter app.
* The dataset is of dimensions $35,77,296\times87$. There are $35,77,296$ instances of data and there are $87$ columns in each instance.<br/>
A summary of all the columns present in the dataset:<br/>

| S.No | Attribute Name | Description | Attribute Type | unique count |
| --- | --- | --- | --- | --- | 
| 1 | Flow.ID| A unique Id assigned to each of the IP flow captured| Nominal  | 1522917|
| 2 | Source.IP| IP address of the source device | Nominal  | 6566|
| 3 | Source.Port| Port number used by the source device | Numeric | 40519|
| 4 | Destination.IP|  IP address of the destination device | Nominal  | 22824|
| 5 | Destination.Port| Port number used by the destination  | Numeric | 34811|
| 6 | Protocol| Transport layer protocol number (TCP = 6, UDP = 17) | Nominal  | 3|
| 7 | Timestamp| The instant the packet was captured stored in the next date format: Dd/mm/yyyy HH:MM:SS | Nominal  | 41915|
| 8 | Flow.Duration| The total duration of the flow | Numeric | 2044412|
| 9 | Total.Fwd.Packets| The total number of packets in the forward direction | Numeric | 8530|
| 10 | Total.Backward.Packets| The total number of packets in the backward direction | Numeric | 8905|
| 11 | Total.Length.of.Fwd.Packets| The total length of forward packets in bytes | Numeric | 104568|
| 12 | Total.Length.of.Bwd.Packets| The total length of backward packets in bytes | Numeric | 223090|
| 13 | Fwd.Packet.Length.Max| Maximum length of forward packet in bytes | Numeric | 7737|
| 14 | Fwd.Packet.Length.Min| Minimum length of backward packet in bytes | Numeric | 1761|
| 15 | Fwd.Packet.Length.Mean| Mean value in bytes of all the packet length in forward Direction | Numeric | 422885|
| 16 | Fwd.Packet.Length.Std| The standard deviation in bytes of all forward packets | Numeric | 1220764|
| 17 | Bwd.Packet.Length.Max| The maximum value in bytes of the packet length in the backward direction. | Numeric | 12167|
| 18 | Bwd.Packet.Length.Min| The minimum value in bytes of the packet length in the backward direction. | Numeric | 1491|
| 19 | Bwd.Packet.Length.Mean| The mean value in bytes of the packet length in the backward direction. | Numeric | 561062|
| 20 | Bwd.Packet.Length.Std| The standard deviation in bytes of the packet length in the backward direction. | Numeric | 1224601|
| 21 | Flow.Bytes.s| The number of bytes per second in the flow. | Numeric | 2386542|
| 22 | Flow.Packets.s| The number of packets per second in the flow. | Numeric | 2352220|
| 23 | Flow.IAT.Mean| The mean value of the inter-arrival time of the flow (in both directions). | Numeric | 2329076|
| 24 | Flow.IAT.Std| The standard deviation of the inter-arrival time of the flow (in both directions). | Numeric | 2450818|
| 25 | Flow.IAT.Max| The maximum value of the inter-arrival time of the flow (in both directions). | Numeric | 1724972|
| 26 | Flow.IAT.Min| he minimum value of the inter-arrival time of the flow (in both directions). | Numeric | 104891|
| 27 | Fwd.IAT.Total| The total Inter-arrival time in the forward direction. | Numeric | 1896396|
| 28 | Fwd.IAT.Mean| The mean inter-arrival time in the forward direction. | Numeric | 2091594|
| 29 | Fwd.IAT.Std| The standard inter-arrival time in the forward direction. | Numeric | 2167212|
| 30 | Fwd.IAT.Max| The maximum value of the inter-arrival time in the forward direction. | Numeric | 1642105|
| 31 | Fwd.IAT.Min| The minimum value of the inter-arrival time in the forward direction. | Numeric | 175655|
| 32 | Bwd.IAT.Total| The total Inter-arrival time in the backward direction. | Numeric | 1657080|
| 33 | Bwd.IAT.Mean| The mean inter-arrival time in the backward direction. | Numeric | 1986588|
| 34 | Bwd.IAT.Std|  The standard inter-arrival time in the backward direction. | Numeric | 2107991|
| 35 | Bwd.IAT.Max| The maximum value of the inter-arrival time in the backward direction. | Numeric | 1298206|
| 36 | Bwd.IAT.Min| The minimum value of the inter-arrival time in the backward direction. | Numeric | 149050|
| 37 | Fwd.PSH.Flags| The number of times the packets sent in the flow had the pushing flag bit set as 1 in the forward direction. | Numeric | 2|
| 38 | Bwd.PSH.Flags| The number of times the packets sent in the flow had the PSH (pushing) flag bit set as 1 in the backward direction. | Numeric | 1|
| 39 | Fwd.URG.Flags| The number of times the packets sent in the flow had the URG (Urgent) flag bit set as 1 in the forward direction. | Numeric | 1|
| 40 | Bwd.URG.Flags| The number of times the packets sent in the flow had the URG (Urgent) flag bit set as 1 in the backward direction. | Numeric | 1|
| 41 | Fwd.Header.Length| The header length of the packets flow in the forward direction. | Numeric | 21914|
| 42 | Bwd.Header.Length| The header length of the packets flow in the backward direction. | Numeric | 22977|
| 43 | Fwd.Packets.s| The number of packets per second in the forward direction. | Numeric | 2293417|
| 44 | Bwd.Packets.s| The number of packets per second in the backward direction. | Numeric | 2190615|
| 45 | Min.Packet.Length| The minimum length of the packets registered in the flow (both forward and backward directions). | Numeric | 1096|
| 46 | Max.Packet.Length| The maximum length of the packets registered in the flow (both forward and backward directions). | Numeric | 12451|
| 47 | Packet.Length.Mean|  The mean value of the length of the packets registered in the flow (both forward and backward directions). | Numeric | 810255|
| 48 | Packet.Length.Std| The standard deviation of the length of the packets registered in the flow (both forward and backward directions). | Numeric | 1674168|
| 49 | Packet.Length.Variance| The variance of the length of the packets registered in the flow (both forward and backward directions). | Numeric | 1669723|
| 50 | FIN.Flag.Count| The number of times the packets sent in the flow had the FIN flag bit set as 1.  | Numeric | 2|
| 51 | SYN.Flag.Count| The number of times the packets sent in the flow (in both directions) had the SYN (Synchronize) flag bit set as 1. | Numeric | 2|
| 52 | RST.Flag.Count| The number of times the packets sent in the flow (in both directions) had the RST (Reset) flag bit set as 1 - (An RST says reset the connection.) | Numeric | 2|
| 53 | PSH.Flag.Count| The number of times the packets sent in the flow (in both directions) had the PSH (Pushing) flag bit set as 1. | Numeric | 2|
| 54 | ACK.Flag.Count| The number of times the packets sent in the flow (in both directions) had the ACK (Acknowledged) flag bit set as 1.  | Numeric | 2|
| 55 | URG.Flag.Count| The number of times the packets sent in the flow (in both directions) had the URG (Urgent) flag bit set as 1 | Numeric | 2|
| 56 | CWE.Flag.Count| The number of times the packets sent in the flow (in both directions) had the CWR (Congestion Window Reduced) TCP flag set as 1. | Numeric | 1|
| 57 | ECE.Flag.Count| The number of times the packets sent in the flow (in both directions) had the ECE (Explicit Congestion Notification Echo) TCP flag set as 1. | Numeric | 2|
| 58 | Down.Up.Ratio| Download and upload ratio. | Numeric | 48|
| 59 | Average.Packet.Size| The average size of each packet. Packet Size specifies only the size of the header on the packet. | Numeric | 805227|
| 60 | Avg.Fwd.Segment.Size| The average segment size observed in the forward direction. | Numeric | 422626|
| 61 | Avg.Bwd.Segment.Size| Average Segment size observed in the backward direction. | Numeric | 560889|
| 62 | Fwd.Header.Length.1| The header length of the packets flow in the forward direction. | Numeric | 21914|
| 63 | Fwd.Avg.Bytes.Bulk| The average number of bytes bulk rate in the forward direction.Bulk data transfer is a software-based mechanism designed to move large data file using compression, blocking and buffering methods to optimize transfer times. | Numeric | 1|
| 64 | Fwd.Avg.Packets.Bulk| Average number of packets bulk rate in the forward direction. | Numeric | 1|
| 65 | Fwd.Avg.Bulk.Rate| Average number of bulk rate in the forward direction. | Numeric | 1|
| 66 | Bwd.Avg.Bytes.Bulk| Average number of bytes bulk rate in the backward direction. | Numeric | 1|
| 67 | Bwd.Avg.Packets.Bulk| Average number of packets bulk rate in the backward direction. | Numeric | 1|
| 68 | Bwd.Avg.Bulk.Rate| Average number of bulk rate in the backward direction. | Numeric | 1|
| 69 | Subflow.Fwd.Packets| The average number of packets in a subflow in the forward direction. | Numeric | 8530|
| 70 | Subflow.Fwd.Bytes| The average number of bytes in a subflow in the forward direction. | Numeric | 104568|
| 71 | Subflow.Bwd.Packets| The average number of packets in a subflow in the backward direction. | Numeric | 8905|
| 72 | Subflow.Bwd.Bytes| The average number of bytes in a subflow in the backward direction. | Numeric | 223090|
| 73 | Init_Win_bytes_forward| The total number of bytes sent in the initial window in the forward direction. TCP uses a sliding window flow control | Numeric | 20139|
| 74 | Init_Win_bytes_backward| The total number of bytes sent in the initial window in the backward direction. | Numeric | 20670|
| 75 | act_data_pkt_fwd| Count of packets with at least one byte of TCP data payload in the forward direction. | Numeric | 7609|
| 76 | min_seg_size_forward| Minimum segment size observed in the forward direction. | Numeric | 9|
| 77 | Active.Mean|  The mean time a flow was active before becoming idle. | Numeric | 653020|
| 78 | Active.Std| Standard deviation time a flow was active before becoming idle. | Numeric | 518682|
| 79 | Active.Max|  Maximum time a flow was active before becoming idle. | Numeric | 589454|
| 80 | Active.Min| Minimum time a flow was active before becoming idle. | Numeric | 340623|
| 81 | Idle.Mean| Mean time a flow was idle before idle before becoming active. | Numeric | 825302|
| 82 | Idle.Std| Standard deviation time a flow was idle before becoming active. | Numeric | 570416|
| 83 | Idle.Max|  The maximum time a flow was idle before becoming active. | Numeric | 702678|
| 84 | Idle.Min| The minimum time a flow was idle before becoming active. | Numeric | 783592|
| 85 | Label| The state of the flow (benign or malign). | Nominal  | 1|
| 86 | L7Protocol| This attribute represents the code number of the layer 7 protocol as obtained from nDPI in Ntopng application. | Nominal  | 78|
| 87 | ProtocolName| This attribute is the objective class of the dataset. | Nominal  | 78|


###  Task 1
#### EDA Findings and Visualizations
**Data visualiations**:
![HeatMapNumericColumns](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/ec5bea08-d486-4cec-81ec-f3556152a3ae)

![scatterPlotNumericColumns](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/4a6d03a8-f121-463f-8712-0140dbdc6b0a)

![ProtcolDistribution](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/93a6f08e-04aa-419a-a987-d976256a790f)

![DatewiseDistribution](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/eb9f6dd9-24fb-43e9-be6d-99cf76642e19)

![download](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/9e0b7524-47c4-4e98-a728-f2bb95710a85)
![image](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/bc45390b-63fb-472c-abe9-64943a6e179c)

![SourceIPCoounts](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/5a3df0c7-70b6-4821-ad4c-35a7d0a8e5fa)

![DestIpCounts](https://github.com/Gangaraj-eng/IT496_DataForce_CourseProject1/assets/77287821/61716965-efd1-4d03-a695-b882ca90565e)

**Findings From  EDA**:
1. Most of the attributes are of numeric type, except a few nominal attributes like ProtocolName, Label, Source and destination IP addresses, and timestamp.
2. There are no such null or missing values in the given dataset as it is collected through software
3. Most of the columns have a right-skewed distribution
4. Most of the ip flows are using Google Protocol followed by HTTP and HTTP_Proxy as the layer 7 protocol
5. Almost 90% of IP flows are using TCP with a few using UDP as Transport Layer protcol
6. There are few columns having only a single unique value for all instances.
7. Among the 6 days on which data is recoreded, 27th april has the highest number of flows recoreded
8. Many sets of columns have a similar correlation among them and thus there is a scope for dimensionality reduction to reduce the columns for computational efficiency

### Task 2
#### Classification problems
The following classification problems can be analysed for the following dataset:
1. **Application layer protocol identification**: Based on the network flow details, the task is to classify which application layer protocol, the given flow used, based on attributes like number of forward and backward packets, flags used, forward and backward segments and so on.
2. **Transport layer protocol identification**: Similarly we can classify the transport layer protcol number used in the flow as TCP(6) or UDP(17) by analysing the numerical information about forward and backward packets, flags used, and so on.<br/>

    Among these, problem 1 - Application layer protocol identification seems most interesting as there are more number of classes compared to other problems and the distribution of dataset is more balanced compared to Transport layer protocol(where 90% of data belongs to one of the classes). This is not the case for application layer protocol and more better classification analysis is possible.


