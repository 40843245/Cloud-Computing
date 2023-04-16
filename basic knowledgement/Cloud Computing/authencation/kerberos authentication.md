# Kerberos Authentication
## Intro
Kerberos authentication is an authentication protocol that is used to verify the identity of a user or host. 

## Benefit
The benefits gained by using Kerberos for domain-based authencations are:
      
      1)Delegated authentication
      2)Single sign on
      3)Interoperability
      4)More efficient authentication to servers
      5)Mutual authentication
  
For more details, visit MSDS which is given in ref section .

## Application
Take a company Cloud-era as an example.

Clould-era is an American company for Cloud Computing.

It develops Cloud-era distributed Hadoop which supports strong Kerberos authenications.

It can do the following things.

      1)Prevent malicious user impersonation.
      2)Enforce user authentication on all RPCs (remote procedure calls).
      3)Prevent user manipulation of group membership by performing group resolution on the Hadoopmaster nodes, cluster nodes and job tracker.
      4)Ensure proper isolation as map tasks are run under the account of the user who submitted the job.

![image](https://user-images.githubusercontent.com/75050655/232261673-e9a9ff31-e8cb-4889-b810-6547bf2a6ffb.png)

## Ref

MSDS:

https://learn.microsoft.com/en-us/windows-server/security/kerberos/kerberos-authentication-overview
