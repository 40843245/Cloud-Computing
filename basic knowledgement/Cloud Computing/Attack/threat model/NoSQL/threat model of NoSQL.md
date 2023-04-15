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


## Inefficient Authorization Mechanisms
## Susceptibility to Injection Attacks
## Lack of Consistency
## Insider Attacks
