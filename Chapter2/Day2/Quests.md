 1.  `changeGreeting` is called to change the state of a smartcontract and we know that scripts are used for viewing the state of smartcontract so we keep them separate.
      Note: Hey I tried putting the `changeGreeting` in script and it changed the value in console. So does that the mean the state of blockchain chenged and does it cost gas fee?
      ![image](https://user-images.githubusercontent.com/90955843/155646240-2fd975c6-566e-4a84-8e1d-e8db5f41e4d4.png)
      
 2.  `AuthAccount` refers to the account whose data is being accessed for making a transaction.

 3.  Both phases are used to change the state of blockchain by transaction.`prepare` phase  can access data in an account for an transaction but an `execute` phase annot access
     the data in your account. Separation between the phases is purely logical.
 
 4. https://play.onflow.org/64002da0-a63c-4966-8034-8b999cb62ccc?type=account&id=cdeaba15-21ea-42b7-b1f7-e911efbd0348&storage=none  
   ![image](https://user-images.githubusercontent.com/90955843/155827586-9365ee7d-da8f-4dd0-971e-afc7be1dea07.png)

 

