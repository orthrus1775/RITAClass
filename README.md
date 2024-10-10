# RITA Class Lab 2  

## Understanding RITA UI  
Destination: Limited character width, if it is cut off you will need to look in zeek logs, or view in csv (rita view <dataset> --stdout)  
Beacon: Probability of a beacon  
Duration: lenght of time system was communicating with the destination  
Subdomains: Will show subdomains most associated with C2 over DNS  
Prevalence: How many diffrent systems are talking to the destination, more effective with live capture  
First Seen: When it was first seen, more effective with live capture (Max is 90 days)  
MIME Type Mismatch: Client downloaded a file from the server and the MIME type offered by the server does not match the file provided, url has .jpg but sending .txt file  
Rare Signature: User agent string only being used on the system when talking with destination. Should have consistant user agent strings when using a browser    

## Import a PCAP  
Execute the following commands  
```bash
zeek readpcap ~/pcaps/lab2.pcap ~/labs/lab2/
```  
```bash
rita import -l ~/labs/lab2/ -d lab2
```
```bash
rita view
```
```bash
rita list
```  
```bash
rita view lab2
```  

***Type Ctl+C to exit the RITA UI***    


## Questions  
1. What is the probability of the beacon?  

2. What is the connection count?  

3. What is the likely operating system of the source IP?  

4. Are there any port, protocol, or service mismatches?  

5. What further questions would you ask based on the data provided?  

6. What should the `-d` flag name not end with?  

7. If you had a many custom configurations and/or threat intel feed you would like use in your analysis, what flag would you use? Would that flag work if the data was already imported?  



[PCAP Source](https://github.com/nipunjaswal/networkforensics/blob/master/Ch7/Empire/empire.pcap)


