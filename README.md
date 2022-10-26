# KafkaBasics

## 1. Kafka Architecture

![image](https://user-images.githubusercontent.com/114802910/197870935-f2da18ab-6bad-4f33-8678-9079df1a4e3e.png)


## 2. Apache Kafka Key Terminologies:

**1. Producer**

     An application that sends data/message to Kafka.
   
**2. Consumer**
  
     An application that retrieves or consumes data from Kafka.


**3. Broker**

     Broker is referred to as Kafka Server. By default Kafka stores data for 2 weeks and it can be extended via admin permissions
   
   
**4. Cluster**

     Clusters are group of computers sharing the workload of kafka servers. Kafka is a distributed system. A Kafka cluster is a system that consists of several Brokers, Topics, and Partitions.
   
   
**5. Topic**


    Kafka Topics are Virtual Groups or Logs that hold messages and events in a logical order. Topic is a unique name for the dataset getting stored in kafka server.
   
**6. Partitions**

     PArtitions are use to store big Kafka Topic, by dividing it inot smaller logs and store it separately inside once cluster.
     With Kafka Partitions, one can effectively divide Kafka Topic to distribute them across different Kafka Servers in the Kafka cluster.
     Even if one of the Servers fail in the future, the messages will be present across other Kafka Servers, eliminating the permanent loss of data

**7. Offset**
   
     Unique Id given to message as they arrive in a partition. This number once assigned cannot be changed. First message gets an offset 0 the next one gets 1 and so on. Global unique Identifier for locating a message is " Topic Name -> Partition Number -> Offset" . With these 3 info one can track the message in kafka.
     
**8. Consumer groups**

    A group of consumers acting  as a single logical unit. Just like there are multiple brokers inside one kafka cluster to distribute the load. similarly at consumer side we have consumer groups to distribute the load of such huge data incoming from kafka server. Partitionng and Consumer group are ways to increase the scalability.
    
    
![image](https://user-images.githubusercontent.com/114802910/198100408-cd4a28b6-37f3-4e59-b4de-2c4530a45003.png)



