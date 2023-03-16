# NoSQL
## Category
1. BigTable : It was developed by Google in 2004 and is now used in more than 60 Google applications such as Google Earth, Web Indexing, Google Financing, Google Analytics and Personalized search.
2. Cassandra : one of the most known engines for NoSQL. 
3. DynamoDB : It was developed by Amazon to support its applications.
4. HBase : It is scalable and fault-tolerantand  performs atomic row operations with row level-locking ,featuring compression and in-memory. 
5. Hypertable :

## Details of them

### BigTable
#### Feature
The system is 
      
      distributed,
      high efficient and
      proprietary 
      
to manage structured data.

Since it  organizes tables as different  groups of columns 
with variable dimensions and consisting  in a sparse, distributed, persistent, multidimensionalsorted  map.

![image](https://user-images.githubusercontent.com/75050655/225528340-b48c06a1-072f-461a-a4c8-9301fe48b89c.png)

### Cassandra
#### Feature

It supplies <b>high performance </b> at <b>massive scale</b> and <b>high availability</b>

since it uses a peer-to-peer (P2P) distributed architecture (see PS.1)

that is much more elegant, easy to set  up and maintain and has no single point-of-failure.

That is, when a node dies, other nodes can connect each other.

Cassandra implements a hierarchical architecture based on columns (name, value and timestamp) grouped by families that map the columns in each line.

### DynamoDB
#### Feature

The system meets these requirements
      
      high  reliability and
      high availability
  
It uses data partioning and replicates data by consistent hashing. (PS.2)

During updates, the consistency is maintained using the <b>quorum-like</b> technique. (PS.3)

Additionally, it decenteralized replica synchronization protocol.

On top of that, DynamoDB also provides fault detection to be added and removed without any manual partitioning and distribution.

### HBase
#### Feature
This systemis a sparse, multidimensional, sorted map in which each cell is uniquely identified by row id, column  id and timestampset. 


### Summary
#### Comparison of these system
![image](https://user-images.githubusercontent.com/75050655/225613442-5bb92b9a-ee8a-4b54-82f9-c230632cf731.png)



### PS.1
In P2P model, you can think that each user is a node where its degree is at least 2.

A P2P model should look like this.

![image](https://user-images.githubusercontent.com/75050655/225529785-c298c5e9-25be-4289-9164-76ae77e994f7.png)


If one node dies (shown as following figure), then other nodes can connect each other.

![image](https://user-images.githubusercontent.com/75050655/225530594-d69a30a1-6844-4b93-b0f1-13dfb724c4ab.png)

Although it has many advantages, 

it has critical disadvantages.

The reference simply talk about P2P network.

https://www.geeksforgeeks.org/what-is-p2ppeer-to-peer-process/

![image](https://user-images.githubusercontent.com/75050655/225531290-faae9f6e-0e57-43ca-9c3a-bbc9f10aeb54.png)

### PS.2
Introduction to consistent hashing.

https://medium.com/swlh/consistent-hashing-68c13951083e

### PS.3

Introduction to <b>quorum-like</b> technique.

English version:

https://en.wikipedia.org/wiki/Quorum_%28distributed_computing%29

Chinese version:

https://zh.wikipedia.org/zh-tw/Quorum_(%E5%88%86%E5%B8%83%E5%BC%8F%E7%B3%BB%E7%BB%9F)
