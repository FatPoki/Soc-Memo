![[Pasted image 20260204233801.png]]

Splunk is a network log monitoring framework that make it fairly easy for us to check logs.

### **index=main**

> **Is used to mention the index which contains our uploded file.**

  ### **source="sample.csv"  host="web0"** 
  

>**Index source host are some ways by which we clearly select our required file from the large file pool of splunk .**


we use it as :  index="main" source="sample.csv" host="web0" 
in filter section.

*  Because the result are really long and messy we use some other filter to see better and clean results.

```
index="main" source="data.csv" host="web0" password
| table _time host src_ip _raw 

```


###  |  ( pip char)

**Is used to work on output of prev query and take it as base for current input.**

  ###  **'_ _time'** 

**Is a placeholder for time in data file that tells about the time and date of an event.**

### host 

**Just like _time placeholder we have host  , src_ip and _raw  which show details of host of system , source ip , raw data executed by client as of file, respectively.**
### _raw

**a default, hidden field containing the original, unparsed text of an event as it was ingested**
  

### password

**password is a keyword that is used as a filter in splunk filter field ,** 
**this will show me only query that have password term in them,** 

**we can also use failed , ssh , login ,forget or any other to get custom filter result,**


___

we can execute table query and toggle from gui view and see starting point packet request all in a sequence so it will be easy to understand IOC.

* Combine head , tail , and , or , not , * for better results we can also use regx