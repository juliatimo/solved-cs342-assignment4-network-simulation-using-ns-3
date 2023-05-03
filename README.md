Download Link: https://assignmentchef.com/product/solved-cs342-assignment4-network-simulation-using-ns-3
<br>
In this assignment you need to simulate a computer network for a given application using the discrete event network simulator <strong>ns-3</strong>. You can download the software and documentation of <strong>ns-3</strong> from the website <a href="https://www.nsnam.org/">https://www.nsnam.org</a><a href="https://www.nsnam.org/">.</a> The assignment will be solved in groups where each group, comprised of 3 members, needs to work on an application assigned to it. The applications’ network specifications, the required experiments, and related questions are given in pages 2-7 of this document. Follow the general instructions given below and any specific instructions mentioned in the application description.

<strong>General Instructions: </strong>

<ol>

 <li>Each group needs to simulate one application assigned to them and make one single submission on Moodle. <strong><u>Only one member from a group needs to make the submission</u></strong>. The information about the allocation of applications to groups is contained in <strong>Table 1</strong> given below.</li>

 <li>Install <strong>ns-3</strong> on your computer, write programs and simulate the network described in the given application assigned to you, perform the required experiments, and answer the given questions.</li>

 <li>Use <strong>ns-3</strong>’s <strong>Flow Monitor</strong> module to collect and store the performance data of network protocols from the simulation. <strong>Do not use PCAP + Wireshark for the trace collection</strong>. No marks will be awarded if your application uses PCAP file for trace collection.</li>

 <li>Submit your set of source code files, <strong><u>along with a report clearly mentioning all observations,</u> <u>explanations,</u></strong><u> <strong>containing the graphs, and all the answers</strong></u>, as a zipped file on Moodle. The <strong>ZIP file’s name should be the same as your group number</strong>, for example, “Group_4.zip”, or “Group_4.rar”, or “Group_4.tar.gz<strong>”. <u>Submission without a report will not be awarded any marks.</u></strong></li>

 <li><strong><u>Grading Scheme:</u></strong> Total marks 20. 10 marks for code compilation and execution. 10 marks for answers, observations, and plot analysis in report.</li>

 <li><strong>Write your own source codes and do not copy from any source. Plagiarism and use of unfair means will be penalised by awarding NEGATIVE marks (equal to the maximum marks for the assignment). </strong></li>

</ol>

<strong> </strong>

<strong><u>Table 1: Allocation of applications to groups</u></strong>

<strong> </strong>

<table width="617">

 <tbody>

  <tr>

   <td width="60"><strong>  App ID </strong></td>

   <td width="36"> </td>

   <td width="22"> </td>

   <td width="36"> </td>

   <td width="30"><strong>  </strong></td>

   <td width="29"><strong>G </strong></td>

   <td width="29"><strong>r </strong></td>

   <td width="29">o</td>

   <td width="29">u</td>

   <td width="22">p</td>

   <td width="29"> </td>

   <td width="29">I</td>

   <td width="29">D</td>

   <td width="29">s</td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

  </tr>

  <tr>

   <td width="60">1</td>

   <td width="36">1</td>

   <td width="22">2</td>

   <td width="36">3</td>

   <td width="30">4</td>

   <td width="29">5</td>

   <td width="29">6</td>

   <td width="29">7</td>

   <td width="29">8</td>

   <td width="22">9</td>

   <td width="29">55</td>

   <td width="29">56</td>

   <td width="29">57</td>

   <td width="29">58</td>

   <td width="29">59</td>

   <td width="29">60</td>

   <td width="29">61</td>

   <td width="29">62</td>

   <td width="29">63</td>

   <td width="29"> </td>

  </tr>

  <tr>

   <td width="60">2</td>

   <td width="36">10</td>

   <td width="22"> </td>

   <td rowspan="5" width="36">48</td>

   <td rowspan="5" width="30">49</td>

   <td rowspan="5" width="29">50</td>

   <td rowspan="5" width="29">51</td>

   <td rowspan="5" width="29">52</td>

   <td rowspan="5" width="29">53</td>

   <td rowspan="5" width="22">54</td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

  </tr>

  <tr>

   <td width="60">3</td>

   <td width="36">19</td>

   <td width="22"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

  </tr>

  <tr>

   <td width="60">4</td>

   <td width="36">28</td>

   <td width="22"> </td>

   <td rowspan="3" width="29"> </td>

   <td rowspan="3" width="29"> </td>

   <td rowspan="3" width="29"> </td>

   <td rowspan="3" width="29"> </td>

   <td rowspan="3" width="29"> </td>

   <td rowspan="3" width="29"> </td>

   <td rowspan="3" width="29"> </td>

   <td rowspan="3" width="29"> </td>

   <td width="29"> </td>

   <td width="29"> </td>

  </tr>

  <tr>

   <td width="60">5</td>

   <td width="36">37</td>

   <td width="22"> </td>

   <td width="29"> </td>

   <td width="29">82</td>

  </tr>

  <tr>

   <td width="60">6</td>

   <td width="36">46</td>

   <td width="22">47</td>

   <td width="29"> </td>

   <td width="29"> </td>

  </tr>

 </tbody>

</table>




<strong>Application #1:</strong>

Analyse and compare TCP Hybla, TCP Westwood+, and TCP YeAH-TCP performance. Select a Dumbbell topology with two routers R1 and R2 connected by a (10 Mbps, 50 ms) wired link. Each of the routers is connected to 3 hosts, i.e. H1, H2, H3 (i.e. senders) are connected to R1, and H4, H5, H6 (i.e. receivers) are connected to R2. The hosts are attached with (100 Mbps, 20 ms) links. Both the routers use drop-tail queues with queue size set according to bandwidth-delay product. Senders (i.e. H1, H2 and H3) are attached with TCP Hybla, TCP Westwood+, and TCP YeAH-TCP agents, respectively. Choose a packet size of 1.3 KB and perform the following tasks. Make appropriate assumptions wherever necessary.




<ol>

 <li>Start only one flow and analyse the throughput over sufficiently long duration. Mention how you select the duration. Plot the evolution of congestion window w.r.t. time. Perform this experiment with all the flows attached to all the three sending agents.</li>

 <li>In the next experiment, start 2 other flows sharing the bottleneck while the first one is in progress and measure the throughput (in Kbps) of each flow. Plot the throughput and evolution of the TCP congestion window for each of the flow at a steady-state. Report the maximum throughput observed for each of the flows.</li>

 <li>Measure the congestion loss and the goodput over the duration of the experiment for each of the flows.</li>

</ol>

<strong> </strong>

<strong>Application #2:</strong>

Compare the performance of TCP over wired and wireless networks. Consider a topology as described below. The network consists of two TCP sources Node0 and Node2, corresponding to two TCP destinations Node1 and

Node3 respectively. Node2 and Node3 come in wired domain with two routers R1 and R2 (connected by a {10 Mbps, 50 ms} wired link) between them. Both the routers use drop-tail queues with queue size set according to bandwidth-delay product. Node0 comes in domain of Base Station 1 (BS1) and Node1 comes in domain of Base Station 2 (BS2). BS1 and BS2 are connected by a (10 Mbps, 100 ms) wired link.  The hosts, i.e. Node0, Node1, Node2, Node3 are attached with (100 Mbps, 20ms) links to routers or base stations (as shown in the figure below). The sources (Node0 and Node2)) use three TCP agents (i.e. TCP Westwood, TCP Veno and TCP Vegas) to generate three different TCP flows. Study and plot the fairness index (Jain’s fairness index) and throughput change when the TCP packet size is varied; all the other parameter values are kept constant. You should use the following TCP packet size values (in Bytes): 40, 44, 48, 52, 60, 552, 576, 628, 1420 and 1500 for your experiments. The throughput (in Kbps) and fairness index must be calculated at steady-state. Make appropriate assumptions wherever necessary.                <strong> </strong>

<strong>Application #3:</strong>

Create a topology of two nodes N0 and N1 connected by a link of bandwidth 1 Mbps and link delay 10 ms. Use a drop-tail queue at the link. Set the queue size according to bandwidth-delay product. Create a TCP agent (type of the agent specified below) and FTP traffic at N0 destined for N1. Create 5 CBR traffic agents of rate 300 Kbps each at N0 destined for N1. Make appropriate assumptions wherever necessary. The timing of the flows are as follows:

<ul>

 <li>FTP starts at 0 sec and continues till the end of simulation.</li>

 <li>CBR1 starts at 200 ms and continues till end.</li>

 <li>CBR2 starts at 400 ms and continues till end.</li>

 <li>CBR3 starts at 600 ms and stops at 1200 ms.</li>

 <li>CBR4 starts at 800 ms and stops at 1400 ms.</li>

 <li>CBR5 starts at 1000 ms and stops at 1600 ms.</li>

 <li>Simulation runs for 1800 ms.</li>

</ul>

<ol>

 <li>Plot graph(s) of TCP congestion window w.r.t. time for following 5 TCP congestion control algorithm implementations, and describe the TCP congestion control algorithms’ behaviour.

  <ul>

   <li>Case 1: use TCP New Reno</li>

   <li>Case 2: use TCP Hybla</li>

   <li>Case 3: use TCP Westwood</li>

   <li>Case 4: use TCP Scalable</li>

   <li>Case 5: use TCP Vegas</li>

  </ul></li>

 <li>Draw a graph showing cumulative TCP packets dropped w.r.t. time comparing above 5 TCP congestion control algorithm implementations.</li>

 <li>Draw a graph showing cumulative bytes transferred w.r.t. time comparing above 5 TCP congestion control algorithm implementations.</li>

</ol>

<strong> </strong>

<strong>Application #4:</strong>

Compare the effect of buffer size on TCP and UDP flows. Select a Dumbbell topology with two routers R1 and R2 connected by a (10 Mbps, 100 ms) link. Each of the routers is connected to 3 hosts, i.e. H1, H2, H3 are connected to R1, and H4, H5, H6 are connected to R2. All the hosts are attached to the routers with (100 Mbps, 10 ms) links. Both the routers (i.e. R1 and R2) use drop-tail queues with equal queue size set according to bandwidth-delay product. Choose a packet size of 1.5 KB. Start 4 TCP New Reno flows, and after a while start 2 CBR over UDP flows each with 20 Mbps. These flows are randomly distributed across H1, H2 and H3. Increase the rate of one UDP flow up to 100 Mbps and observe its impact on the throughput of the TCP flows and the other UDP flow. Vary the buffer size in the range of 10 packets to 800 packets and repeat the above experiments to find out the impact of buffer size on the fair share of bandwidth and plot the necessary graphs. Make appropriate assumptions wherever necessary.

<strong>Application #5:</strong>

Using the network simulator ns-3, study the characteristics of IEEE 802.11. For the purpose of experiment, use the topology as follows. There are 3 nodes in the network located in a straight line at locations 250*i, with i=0, 1, 2. Node 0 and Node 2 both have TCP traffic to Node 1 (started randomly within 1 to 5 seconds of starting the simulation). Consider TCP Westwood+ or TCP Hybla for the TCP agents at Node 0 and Node 2, respectively. You have to run the simulations and measure the following from the trace output (the averages are taken over all the nodes). Do not use PCAP file for collecting the trace. Use Flow Monitor module in ns-3 for trace collection. <em>No marks will be given if you consider PCAP trace with Wireshark</em>.

<ol>

 <li>Average bandwidth spent in transmitting RTS, CTS, and ACK.</li>

 <li>Average bandwidth spent in transmitting TCP segments and TCP acks.</li>

 <li>Average bandwidth wasted due to collisions.</li>

 <li>TCP throughput (number of acknowledged bytes per unit time) at each node.</li>

</ol>

You have to run the simulations for 50 seconds each with different RTS thresholds (i.e. 0, 256, 512 and 1000 bytes) and TCP segment size of 1000 bytes. You can use scripts for trace file analysis and to plot the results. Make appropriate assumptions wherever necessary.

<strong>Application #6:</strong>

The objective is to compare the effect of CBR traffic over UDP agent and FTP traffic over TCP agent. Consider a TCP agent from TCP HighSpeed, TCP Vegas and TCP Scalable for the FTP traffic. Consider a Dumbbell topology with two routers R1 and R2 connected by a wired link (30 Mbps, 100 ms), and use drop-tail queues with queue size set according to bandwidth-delay product of the link. Each of the routers is connected to 2 hosts, i.e. H1, H2 are connected to R1, and H3, H4 are connected to R2. The hosts are attached to the routers with (80 Mbps, 20ms) links. The CBR traffic over UDP agent and FTP traffic over TCP agent are attached to H1 and H2 respectively. Choose appropriate packet size for your experiments and perform the following:

<ol>

 <li>Compare the delay (in ms) and throughput (in Kbps) of CBR and FTP traffic streams when only one of them is present in the network. Plot the graphs for the delay (in ms) and throughput (in Kbps) observed with different packet sizes.</li>

 <li>Start both the flows at the same time and also at different times. Also, compare the delay (in ms) and throughput (in Kbps) of CBR and FTP traffic streams. Plot the graphs for the delay (in ms) and throughput (in Kbps) observed with different packet sizes.</li>

</ol>

Make appropriate assumptions wherever necessary.


