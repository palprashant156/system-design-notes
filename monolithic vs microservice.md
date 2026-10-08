# Monolithic vs Microservice Architecture

## Monolithic Architecture
In monolithic architecture, all the functions (authentication, payment processing, inventory management, etc.) are packed together in a single unit called a module or a package.

* **Example:** In an e-commerce application, all the functionalities like authentication, payment, inventory, etc., are packed together in a single unit.

### Benefits of Monolithic Architecture:
1. **Easy to develop:** Since all the functionalities are packed together in a single unit, it is easy to develop the application.
2. **Easy to test:** Since all the functionalities are packed together in a single unit, it is easy to test the application.

**Note:** It is not easy to achieve a single point of failure because all the services are inside one.

---

## Microservices Architecture
In microservices architecture, the application is broken down into smaller, independent services that communicate with each other through APIs.

* **Example:** In an e-commerce application, all the functionalities like authentication, payment, inventory, etc., are packed in different services and communicate with each other through APIs.

### Benefits of Microservices Architecture:
1. **Fault tolerance:** Since all the functionalities are packed in different services, if one service fails, the other services can still work properly.
2. **Easy to test:** Since all the functionalities are packed in different services, it is easy to test the application.
3. **Easy to scale horizontally:** Since all the functionalities are packed in different services, it is easy to scale the application.
4. **Easy to deploy:** Since all the functionalities are packed in different services, it is easy to deploy the application.
5. **Less latency.**

**Easy to achieve a single point of failure: False.** Because if one service fails, the other services can still work properly. Let's say 10 GB of data is distributed in 5 machines (each having a capacity of 3 GB), each holding 2 GB. So if one machine fails, the other 4 are still working. But one issue is there: data is lost. For solving this problem, data replication (every machine has one copy) is used. If any one machine fails, then data goes to the replica.

