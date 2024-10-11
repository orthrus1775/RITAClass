# RITA Class Lab 3  
[PCAP Source](https://malware-traffic-analysis.net/2023/02/27/index.html)  
**Required pcaps for labs are in the ~/pcaps directory**  

## Import the PCAP  
Import the lab3.pcap into RITA as lab3
<details>

<summary>Hint</summary>

```bash
zeek readpcap ~/pcaps/lab3.pcap ~/labs/lab3/
```  

```bash
rita import -l ~/labs/lab3/ -d lab3
```  

```bash
rita view lab3
```

</details>

## Questions  
1.  What is the number of entries with a beacon score of greater than or equal to 50%? What command did you use?  

2. What is the prevalence of hosts connecting to 80.47.61.240? How many hosts can we assume are within the pcap based on this information?  

3. With out further information what questions would you ask about 20.90.156.32?  

4. How many entries have a duration of less than ten seconds? How long after the capture did the connection occur? 

5. Did all the hosts identified in question four connect to the destionation? Based on this information would you investigate these connection further why or why not?  

