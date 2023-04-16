# threat model of NoSQL
There are six major scenarios in the threat model of NoSQL database.

## Transactional Integrity
Let's review the term Integrity and Transaction.

Integrity refers the completeness and realness.

Transaction refers an input data to computer system which is dealt with a single unit of work.

One of the most visible of NoSQL is its soft approach towards ensuring transaction integrity. 

Which means that introducing complex integrity constraint into its architecture will fail NoSQL's primary objective of attaining

better performance and scalability.

Technique such as ATAM (Architectural Trade-off Analysis Method) specificially deal with trade-off in quality requirements in architecural decision.

(such as performance v.s. security)

## Lax Authentication Mechanisms
Across the board, NoSQL uses weak authentication techniques and weak password storage mechanisms. 

This exposes NoSQL to replay attacks and password brute force attacks, resulting in information leakage. 

Additionally, NoSQL uses HTTP Basic-based authentication or Digest-based authentication, which are prone to replay attack 

or man-in-the-middle attack.

REST, which is another preferred communication protocol, is also based on HTTP and is prone to cross-site scripting, 

cross-site request forgery, injection attacks, etc.

Above all, NoSQL does not support integrating third-party pluggable modules to enforce authentication. 

## Inefficient Authorization Mechanisms

Authorization techniques differ from one NoSQL solution to another. 

Most of the popular solutions apply authorization at higher layers rather than enforcing authorization at lower layers. 

More specifically, authorization is enforced on a per-database level rather than at the collection level.  

There is no role-based access control (RBAC) mechanism built into the architecture because 

it is impossible to define user roles and security groups with an RBAC mechanism.

## Susceptibility to Injection Attacks
To have more understanding of Injection Attacks,

recall that SQL commands consist of strings. i.e. Every SQL command is stored as a string.

In my previous note (published in GitHub), the topic about SQL injection have been disccussed.

(If you don't know what it is, you can see my previous note.)

SQL suffers from SQL injection while NoSQL suffers not only SQL injection but also JSON injection, array injection

, view injection, REST injection, GQL injection, schema injection etc. 

## Lack of Consistency

The inability to simultaneously enforce all three elements of the CAP theorem 

(consistency,   availability,andpartition   tolerance)   while   in  distributed  mode  undermines  the trustworthiness  of  the  churned  results. 

As a result, users are not guaranteed consistent results at any given time, 

as each participating node may not be entirely synchronized with the node holding the latest image.  

Current  hashing  algorithms  entrusted to replicate data across the cluster nodes crumple in the event of a single node failure, 

resulting in load imbalance among the cluster nodes.

## Insider Attacks
Lenient security mechanisms can be leveraged to achieve insider attacks. 

These attacks could remain unnoticed because of poor logging and log analysis methods, 

along with other rudimentary security mechanisms. 

As critical data is stowed away under a thin security layer,

it is difficult to ensure that the data owners maintain control.
 
## Ref
https://ulearn.nfu.edu.tw/course/10459/learning-activity/full-screen#/42890
