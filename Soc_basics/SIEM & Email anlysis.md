
### Security information and Event management ( SIEM)

Siem is a centralized platform which allows us to collect , correlates and analyze security data from across an entire IT infrastructure.

**Log source:**  log source is any system that generate logs like, Active directory , FIrewall . Endpoint.

---

###  Splunk Basics

> Splunk is a popular SIEM  platform that  uses SPL( Search Processing Language) to query data
> basic search : we start by spesifying the source like, 


 ```
 
 index=main sourcetype=syslog
 
 ```

#### Filter

-  **Keyword :** to serch spesific keyword we need to just search that term like ( error or failed).
  
- **Field-value pairs :** use syntax like ( user="john_doe" or status=404 ) to pinpoint results.

- **Boolean operators :**   combine filter with and or not operators.

-  **Pipe ( | ) :**  use pipe character to pass search resilt to commands for further analysis such as | stats count by user to see activity per person.

---

### Phishing techniques 

1. AI  generated phishing
   
2. Quishing ( QR code phishing )
   
3. Deepfakes : fraud voice message or video .
   
4. Smishing : phishing delivered via messaging app like sms or whatsapp.

---

###  Email Security Protocols

These 3 records work together to prove that an email is legitmate and has not been tampered or spoofed.


1. **SPF  ( Sender Policy Framework ) :**  A list of authorised ip and domain that are allowed to send you email on your behalf.
      
2.  **DKIM  (Domain Key Identifier mail ) :**   Adds a signature to every outgoing email to make sure that email was not tampered.
   
3. **DMARC ( Domain Based Message Authentication Reporting and Confirmation) : An policy that tells the receiving server what to do in case mail fails SPF or DKIM checks ( eg. reject it or put it in spam)
   
---

### Email Headers

An email header hides plenty of details of sender and receiver that can be used to verify if it is a phishing email or legit.

Always use Bottom - top approach to analyse an email header , 

for example ; 

bottom request 

**i.e**   ==Received: by 2002:a05:7300:7951:b0:62:3ec1:8434 with SMTP id d17csp5155772dyi;==
        ==Sat, 00 Jun 2022 00:00:00 -0700 (PDT)==
        
> This  is our client getting email for first time by source, everything after this is request ongoing.

```


Received: from mta-81-96.sparkpostmail.com (mta-81-96.sparkpostmail.com. [192.174.81.96])
        by mx.google.com with ESMTPS id ji12-  20020a170903324c00b0016163a204cfsi12846642plb.334.2022.06.04.10.17.47
        for <grigori.monaselidze@railsware.com><span style="background-color: inherit;font-family: Menlo, Consolas, monaco, monospace;font-size: inherit"> </span> 
        (version=TLS1_2 cipher=ECDHE-ECDSA-AES128-GCM-SHA256 bits=128/128);
        Sat, 00 Jun 2022 00:00:00 -0700 (PDT)

Received: by 2002:a05:7300:7951:b0:62:3ec1:8434 with SMTP id d17csp5155772dyi;
        Sat, 00 Jun 2022 00:00:00 -0700 (PDT)


```

One can use online email header analysing tools like ``` https://mxtoolbox.com/ ``` 
and others to analyse headers.


>[!info]  
>We can also extract attachment from email and get its hash by ' sha256sum FILE-NAME '





