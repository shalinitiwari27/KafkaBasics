# KafkaBasics

## 1. Kafka Architecture

![image](https://user-images.githubusercontent.com/114802910/197858907-6a9999e4-6fc2-44cc-a7f5-73e637dcb992.png)

## 2. Apache Kafka Key Terminologies:

**1. Producer**

     An application that sends data/message to Kafka.
   
**2. Consumer**
  
     An application that retrieves or consumes data from Kafka.


**3. Broker**

     Broker is referred to as Kafka Server
   
   
**4. Cluster**

     Clusters are group of computers.
   
   
**5. Topic**


    Kafka Topics are Virtual Groups or Logs that hold messages and events in a logical order. 
   
**6. Partitions**

     PArtitions are use to store big Kafka Topic, by dividing it inot smaller logs and store it separately inside once cluster.
     With Kafka Partitions, you can effectively divide Kafka Topic to distribute them across different Kafka Servers in the Kafka cluster.
     Even if one of the Servers fail in the future, the messages will be present across other Kafka Servers, eliminating the permanent loss of data

**7. Offset**
   
     Unique Id for ma message within a partion
     
**8. Consumer groups**

    A group of consumers acting  as a single logical unit


