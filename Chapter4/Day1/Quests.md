1. An account contains:
    * Smart Contract, multiple contracts can be deployed and stored in an account
    * Data, All the data is stored in an account eg: NFT



2. The following are the key difference between `/storage`,`/public` & `/private`.
   * `/storage/` - Only the account owner can access from the `/storage`. All the data lives here.
   * `/public/`  - The information here is accessible to everybody.
   * `/private/` - Only available to the account owner and the people that the account owner gives access to.

3. `.save()` is used to saving the data into the `/storage/`path (account storage).
   `.load()` is used to take the data out from the `/storage/` path (account storage).
   `.borrow()` is used to look the data in the `/storage/` we get the refernce to resource in the account storage here.
   
4. I need to approve the transaction and sign it after that the transaction takes in my `AuthAccount` and you can access the data in your account including saving in it.
   That is there for better security.?

5. 
Smart Contract

![image](https://user-images.githubusercontent.com/90955843/156882296-013d7cf1-e4ac-4307-b6e7-9cfd155dd1e8.png)

Transaction for save and load
![image](https://user-images.githubusercontent.com/90955843/156882224-6b2a27b0-ae3f-4a02-95e1-69172ca4e755.png)

Transaction for save and borrow
![image](https://user-images.githubusercontent.com/90955843/156882204-7f6773fb-6348-4451-96c2-373e575c5a2f.png)

https://play.onflow.org/0fa932ae-7d4b-4f05-9510-fa8f92806f12?type=account&id=d30d546d-70d9-48c9-917e-c70a4a0e58f2&storage=none
