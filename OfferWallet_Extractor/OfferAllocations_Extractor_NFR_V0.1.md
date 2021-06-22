- ## 1. Extractor Name : OfferAllocation Extractor
  - Source system : Multiple systems - > Kafka
  - Micro Service Name : OfferWallet Services
  
    - ### BAU Volumetric 
     - #### TMO Offers
         - No of TMO Offers : < -TBF ->
         - Batch Window Time : < -TBF ->
         
      - #### FPO Offers
         - No of FPO Offers : < -TBF ->
         - Batch Window Time : < -TBF ->         
                       
      - ### Peak Volumetric 
       - #### TMO Offers
         - No of TMO Offers : 10 Million users * 8 offers ==> 80 M offers
         - Batch Window Time : 4 Hours
         
      - #### FPO Offers
         - No of FPO Offers : 6 Million users * 8 offers ==> 48 M offers
         - Batch Window Time : < -TBF ->
