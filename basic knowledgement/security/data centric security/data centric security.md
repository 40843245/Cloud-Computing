# data centric security
## Prequisite
Data centering

## Review
What is data center?

Simply said, data center refers the technique of organizing the data from different user into one or more specific places.

### 3 requirements

A safe data center must make the data be Confidentiality, Integrity, and Availability.

#### Confidentiality
Such as 

    Can unauthorized user access your sensitive data?

#### Integrity
Such as 
    
    Can your data be proven it is own by yourself?

#### Availability
Such as 

     Where can I access my data?
     
     
### Key Concepts
A data-centric security model can follow these 4 basic features.
  
    1)Discover 
    2)Manage 
    3)Protect 
    4)Monitor

#### Discover
    The ability to know where your data is stored.
#### Manage
    The ability to define the access policies to determine who can access the specific data.
#### Protect
    The ability to prevent the unauthorized use of data and prevent sensitive data from being sent to unauthorized users or locations.
#### Monitor
    The constant monitoring of data usage to identify meaningful deviations from normal behaviour that would point to possible malicious intent.
    
### Implementation
From the technical point of view, it repies on the implementation of the following.

![image](https://user-images.githubusercontent.com/75050655/231925125-ed995029-f299-45d1-b892-a97b5320ad36.png)

### Content of Term 
1. Self-describing
2. Self-defending

### Term 
1. Self-describing : 
    
        The data is self-describing means that the data itself can describe the related information. To know information about self-describing data, we don't have to find the other data.
2. Self-defending:
        
        Simply said, a self-defending data refers that the data is embedded that techniques of security (for 3 requirement of security, see above section.).
        
### Technique of data centric security   

In above section, we have discussed the 3 requirements of security -- Confidenitiality, Integrity, and Availability.

Now let's disccuss the approach to achieve the 3 requriements. Let's dig in.

    1)Data access controls and policies.
    2)Encryption
    3)Data masking
    4)Auditing
    5)Privacy-enhancing technologies
#### Data access controls and policies
    It determine who can access specific data. 
    It responds to the element "Management" of 4 key concepts (which have been discussed in above section.)
    
#### Encryption
    If someone access the encrypted data, one can NOT understand what it means unless one has decrypted it successfully.
    A data which is encrypted with a safe cryptography algorithm can ensure that your data is NOT easily to be known by others.
    
    Thus, it also can achieve the 3 requirements.
    
#### Data masking
    The word mask in computer science refers to filter data by specific way, making it NOT seen by others.
    
    Thus, data masking also can achieve the 3 requirements.
    
#### Auditing
    The term data auditing in computer science refers to check the status of the data usage.
    
    With the technique of data auditing, you can check the status of your data usage including it is accessed by unauthorized user.
    
    Thus, it also can achieve the 3 requirements.
    
    It responds to the element "Monitor" of 4 key concepts.
    
#### Privacy-enhancing technologies

    It allows online users to protect the privacy of their personal identifiable information (PII) provided to and handled by services and applications.

### Ref
https://en.wikipedia.org/wiki/Data-centric_security
