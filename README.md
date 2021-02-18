# PaytmLabs SDE Challenge

## Coding Question

Write an interface for a data structure that can provide the moving average of the last N elements added, add elements to the structure and get access to the elements. Provide an efficient implementation of the interface for the data structure.

### Minimum Requirements

1. Provide a separate interface (IE `interface`/`trait`) with documentation for the data structure
2. Provide an implementation for the interface
3. Provide any additional explanation about the interface and implementation in a README file.

## Design Question

Design A Google Analytic like Backend System.
We need to provide Google Analytic like services to our customers. Please provide a high level solution design for the backend system. Feel free to choose any open source tools as you want.

### Requirements

1. Handle large write volume: Billions of write events per day.
2. Handle large read/query volume: Millions of merchants wish to gain insight into their business. Read/Query patterns are time-series related metrics.
3. Provide metrics to customers with at most one hour delay.
4. Run with minimum downtime.
5. Have the ability to reprocess historical data in case of bugs in the processing logic.

### Design Solution

It is important to design application with speed and scalability in mind. While we are implementing the  
application, we should consider important factors such as a lot of processing power, memory, disk space, and redundancy.
It should distribute the load across the several machines for high throghput.

1. We should have proper load balancing mechanism to handle the high volume writes.
2. services based on microservice architecture for horizontal scalability
3. high performance, fault-tolerant distributed streaming platform for asynchronous processing  - Kafka.
4. We can use NoSQL databases for scalability and high performance.
5. Grafana or Knowi or Kibana can be used for historical data representation
