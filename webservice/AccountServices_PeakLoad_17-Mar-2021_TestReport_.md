- ## Summary
    - Test Name :Account Services _Peak Test
    - Test Objective : The test objective is to simulate peak load for the 4 REST API's [Get Charity by Account ID, Get Sparks Account by ID, Get Sparks Account by ID &Identity Type,Sparks Account Creation ]and 1 GraphQL API in Locust POD to POD  [Locut Test Pod to Account Services Pod ] using the cluster end point http://sparks-account-webservice.pluto-perf.svc.cluster.local/account
    - Code Buid :
    - Date and Time : 17-Mar-2021 - 08:03:07 - 17-Mar-2021 - 08:59:27
    - Observations :  The 90% response time for Sparks Account Creation was 11 ms seconds and for all other API's it was less than 6 ms.506 TPS was achieved during the Peak load Test execution. The DB and Account Services CPU utilisation were less than 15%.
    - RAG Status : GREEN
    - PT Bug (if any) : N/A
    - NFR's : [Test NFR](PT_Template_NFR-API.md) [ Provide link to the Test NFR's .md file]
    
 - ## Application-side Metrics
   - ### API Response Time and TPS:
        - #### API Name: Get Charity by Account ID
            -  Pass count:15361
            -  Fail count:0
            -  TPS: 4.8
            -  Average Response Time:5 ms
            -  Median Response Time: 5 ms
            -  90% Response Time: 7 ms
            -  Status : Pass
             
       - #### API Name: Get Sparks Account By ID
            -  Pass count: 420,772
            -  Fail count: 0 
            -  TPS: 120.3
            -  Average Response Time: 5 ms
            -  Median Response Time: 5 ms
            -  90% Response Time: 7 ms
            -  Status : Pass
       - #### API Name: Get Sparks Account By ID & Identity Type
            -  Pass count: 420721
            -  Fail count: 0
            -  TPS: 128.9
            -  Average Response Time: 5 ms
            -  Median Response Time: 5 ms
            -  90% Response Time: 7 ms
            -  Status : Pass
       - #### API Name: Sparks Account Creation 
            -  Pass count: 7726
            -  Fail count: 0
            -  TPS: 2.1 
            -  Average Response Time: 5 ms
            -  Median Response Time: 5 ms
            -  90% Response Time: 11 ms
            -  Status : Pass
       - #### API Name: GraphQL
            -  Pass count: 836510
            -  Fail count: 0
            -  TPS: 249.9
            -  Average Response Time: 5 ms
            -  Median Response Time: 5 ms 
            -  90% Response Time: 7 ms
            -  Status : Pass/ Fail [compare the API test result with NFR and state whether the it has passed or failed.]
   
        
   - ### Response Time Summary :  
        
       ![Response Time - Summary](../Images/ResponseTime_Summary_AccountServices_PeakLoad.png) 
       
  - ## Server-side Metrics 

    - ### Application Server  :
       - NewRelic Dashboard - [NewRelic Dashboard Link](https://gorgon.nr-assets.net/image/8a70c53e-1c72-432a-ab30-2ea4da1cb47a?format=PDF) 
              
    - ### Database Server :
      - CPU and Memory : 
      
      ![Mongo DB CPU and Memory - Sample Image](../Images/MongoDB_Perf_AccountServices_PeakLoad_CPUandMemory_17-Mar-2021.png)
      
      - DB Connections and Queues : 
     
      ![Mongo DB Connections and Queues - Sample Image](../Images/MongoDB_Perf_AccountServices_PeakLoad_QueuesandConnections_17-Mar-2021.png)
      
   
