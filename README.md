# RITA Class Lab 1 

## Login to VM  
SSH to your assigned vm with the following credentials  
- username: analyst
- password: password  

```bash
ssh analyst@X.X.X.X
```  
**Required pcaps for labs are in the ~/pcaps directory**

## Getting to know RITA 
First take a look at the RITA [github](https://github.com/activecm/rita) page and Active Countermeasures [post](https://www.activecountermeasures.com/intro-to-rita-v5/) about RITA  


## RITA files  
Execute the following commands and review the associated files  
```bash
which rita
```  

```bash
rita help
```

```bash
rita import help
```

```bash
ls -GFlash /opt/rita
```  

```bash
ls -GFlash /etc/rita
```

```bash
less config.hjson
```  

```bash
zeek  
```  
We will only be using zeek to import pcaps but it is also capable of live captures.    

## Questions  
1. When someone executes `rita` what is going on in the background?  

2. What are the four things that RITA can do for network traffic analysis? How would these four things enhance our mission execution?  

3. Can you run RITA on the Windows Operating System? How would you integrate RITA, knowing the available SIEM operating systems, into your threat hunt.  

4. What columns support filtering in RITA?  

5. What permissions do you need to use RITA?  

6. What other tool does RITA rely on?  

7. Does RITA support `RFC7303` extensions?  

8. What are the requirments for threat intelligence integration with RITA and what are some things you would need to consider when working in an air gapped environment?  

9. What subnets does RITA filter out when analyizing data? Why would you want to modify the default settings and where would you put your modificaitons?  

10. What is the minimum time in **hours** for `long connections` to recieve a score of high?  

