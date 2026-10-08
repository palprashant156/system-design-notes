In monolithic architecture, 
all the functions (authentication, payment processing, inventory management, etc.) are packed together in a single unit called a module or a package. 

Example - In an e-commerce application, all the functionalities like authentication, payment, inventory, etc. are packed together in a single unit.


Benefits of Monolithic Architecture:

1. Easy to develop: Since all the functionalities are packed together in a single unit, it is easy to develop the application.

2. Easy to test: Since all the functionalities are packed together in a single unit, it is easy to test the application.

**not easy to achive single point of failure becuae all the service are inside one.
In microservices architecture, 
the application is broken down into smaller, independent services that communicate with each other through APIs.

Example - In an e-commerce application, all the functionalities like authentication, payment, inventory, etc. are packed in different services and communicate with each other through APIs.


Benefits of Microservices Architecture:

1. Fault tolerance: Since all the functionalities are packed in different services, if one service fails, the other services can still work properly.

2. Easy to test: Since all the functionalities are packed in different services, it is easy to test the application.

3. Easy to scale horizontally: Since all the functionalities are packed in different services, it is easy to scale the application.

4. Easy to deploy: Since all the functionalities are packed in different services, it is easy to deploy the application.

5. Less latency

easy to achive single point of failure : False, because if one service fails, the other services can still work properly because let say 10 gb of data distrubuted in 5 machine(have capacity of 3gb) each 2gb so if machine fails others 4 still working but one issue is there data is lost for solving this problem data replication(every machine have one copy) is come if any one machine fails then data go on replica.

